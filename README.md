<div align="center">

  <!-- Header Banner -->
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1,11,21&height=220&section=header&text=Nguyen%20Tien%20Dung&fontSize=38&fontColor=ffffff&fontAlignY=38&subtext=ASIC%20Physical%20Design%20(RTL-to-GDSII)&subfontSize=16&subfontAlignY=62" width="100%" alt="Header Banner" />

  <p align="center">
    <img src="https://img.shields.io/badge/Location-Hanoi%2C%20Vietnam-0284c7?style=flat-square&logo=googlemaps&logoColor=white" alt="Location" />
    <img src="https://img.shields.io/badge/Focus-ASIC%20Physical%20Design-8b5cf6?style=flat-square" alt="Focus" />
    <img src="https://img.shields.io/badge/PDK-SkyWater_130nm%20%7C%20GPDK_90nm-10b981?style=flat-square" alt="PDK" />
  </p>

  <p align="center">
    <a href="https://www.linkedin.com/in/vn-ntd" target="_blank">
      <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
    </a>
    &nbsp;
    <a href="mailto:nguyentiendung12022006.vn@gmail.com">
      <img src="https://img.shields.io/badge/Email-nguyentiendung12022006.vn%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
    </a>
  </p>

</div>

---

### 👨‍💻 Giới thiệu

Sinh viên định hướng **ASIC / IC Physical Design (backend)**. Mình đã tự chạy trọn luồng **RTL-to-GDSII** trên SkyWater 130nm bằng OpenLane/OpenROAD, thiết kế và layout mạch custom trên Cadence GPDK 90nm, và viết các công cụ Python để phân tích kết quả (timing, IR-drop, báo cáo PPA).

Dự án nổi bật nhất: lõi RISC-V **PicoRV32** hoàn tất flow tới GDSII, đóng timing ở **133.33 MHz**, Magic DRC = 0, LVS clean. Số liệu và báo cáo gốc đều nằm trong repo để kiểm chứng.

---

### ⭐ Dự án chính: PicoRV32 RTL-to-GDSII (SkyWater 130nm)

[**`riscv_picorv32_sky130_asic_flow`**](https://github.com/vn-ntd/riscv_picorv32_sky130_asic_flow) — flow đầy đủ có GDS, DEF, SPEF, báo cáo signoff và CI.

| Chỉ số | Kết quả (nguồn: `reports/`) |
| :--- | :--- |
| Tần số / Setup slack | **133.33 MHz**, +0.07 ns (post-SPEF, corner tt, 1.8 V, 25 °C) |
| Hold slack | +0.30 ns |
| Core utilization | **69.93%** (die 0.1606 mm²) |
| Magic DRC / TritonRoute DRC | **0 / 0 violations** |
| Netgen LVS | **Clean** (11,317/11,317 nets) |
| Antenna | 21 net còn vi phạm sau global-router repair (đã ghi rõ trong repo) |
| Gate-level simulation | PASS (243 chu kỳ) |
| Công suất (OpenSTA, toggle mặc định) | 45.9 mW @ 133.33 MHz |

**Vấn đề kỹ thuật đã giải quyết**
- `GRT-0119` (nghẽn routing ở utilization 70%): khảo sát PDN, tăng strap pitch 25 → 153.6 µm, khôi phục kênh routing ở M4/M5.
- `DPL-0036` (chèn diode heuristic làm tràn site): bỏ heuristic (3,555 diode), chuyển sang global-router antenna repair (167 diode).

---

### 🧪 Các dự án khác

| Dự án | Nội dung | Loại dữ liệu |
| :--- | :--- | :--- |
| 🧰 [`pd_flow_toolkit`](https://github.com/vn-ntd/pd_flow_toolkit) | Parse báo cáo OpenROAD/Innovus, lint SDC (nhiều rule), so sánh regression giữa 2 lần chạy, sinh dashboard HTML. Có [dashboard thật](https://github.com/vn-ntd/pd_flow_toolkit/blob/main/examples/picorv32_dashboard.html) từ lần chạy PicoRV32. | Công cụ; ví dụ Innovus là dữ liệu mẫu |
| ⚡ [`pdn_analysis_ir_drop`](https://github.com/vn-ntd/pdn_analysis_ir_drop) | Giải MNA cho lưới nguồn, static/dynamic IR-drop, kiểm tra EM, so sánh 4 topology và quét Pareto sụt áp vs nghẽn routing. 35 unit test, CI 3 hệ điều hành. | Mô phỏng, tham số 7nm FinFET generic |
| ⏱️ [`sta_timing_closure_eco`](https://github.com/vn-ntd/sta_timing_closure_eco) | Mô hình STA (NLDM, OCV, CRPR, jitter) và engine ECO tự động. Trên thiết kế mô hình 1.667 GHz: setup WNS −48.97 → +212.73 ps, hold −17.90 → +101.81 ps. | Mô hình giáo dục, thiết kế tự tạo |
| 🔬 [`full_adder_opt`](https://github.com/vn-ntd/full_adder_opt) | Full adder CMOS: bản 36T → bản 28T mirror, layout + RCX trên GPDK 90nm. Diện tích **−37.7%** (90.0 → 56.05 µm²), công suất post-layout **−26.1%**, Assura DRC/LVS clean. | Mô phỏng + layout thật (Virtuoso/Assura) |

---

### 🛠️ Công cụ & Kỹ năng

- **Physical design & signoff:** OpenLane, OpenROAD (TritonCTS, TritonRoute), OpenSTA, Magic, Netgen, KLayout
- **Custom IC (Cadence):** Virtuoso, Spectre, Assura (DRC/LVS/RCX)
- **PDK:** SkyWater 130nm, GPDK 90nm
- **Scripting:** Python, Tcl, Bash, Linux, Git
- **HDL:** Verilog (testbench tự kiểm tra, RTL và gate-level simulation bằng Icarus Verilog)

---

### 📊 GitHub

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=vn-ntd&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117" height="150" alt="GitHub Stats" />
  &nbsp;
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=vn-ntd&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117" height="150" alt="Top Languages" />
</div>

---

<div align="center">
  <sub>© 2026 <b>Nguyen Tien Dung (vn-ntd)</b> • IC Physical Design</sub>
</div>
