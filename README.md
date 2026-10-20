<div align="center">

  <!-- Header Banner -->
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1,11,21&height=220&section=header&text=Nguyen%20Tien%20Dung&fontSize=38&fontColor=ffffff&fontAlignY=38&subtext=ASIC%20%2F%20IC%20Physical%20Design%20Engineer%20%E2%80%A2%20RTL-to-GDSII&subfontSize=16&subfontAlignY=62" width="100%" alt="Header Banner" />

  <!-- Dynamic Typing Subtitle -->
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&pause=1200&color=38BDF8&center=true&vCenter=true&width=620&lines=ASIC+%2F+IC+Physical+Design+Engineer;Full-Flow+RTL-to-GDSII+Implementation;STA+Timing+Closure+(ECO)+%26+Clock+Tree+Synthesis;Power+Integrity+(PDN)+%26+Static+IR-Drop+Analysis;Physical+Verification+(DRC%2FLVS)+on+SkyWater+130nm;EDA+Automation+with+Tcl%2C+Python+%26+Bash" alt="Typing SVG" />
  </a>

  <!-- Meta Badges -->
  <p align="center">
    <a href="https://hits.sh/github.com/vn-ntd/"><img src="https://hits.sh/github.com/vn-ntd.svg?style=flat-square&label=PROFILE%20VIEWS&color=38bdf8" alt="Profile Views" /></a>
    <img src="https://img.shields.io/badge/Location-Hanoi%2C%20Vietnam-0284c7?style=flat-square&logo=googlemaps&logoColor=white" alt="Location" />
    <img src="https://img.shields.io/badge/Specialization-IC%20Physical%20Design%20(ASIC%2FVLSI)-8b5cf6?style=flat-square&logo=microchip&logoColor=white" alt="Specialization" />
    <img src="https://img.shields.io/badge/Target_Node-SkyWater_130nm_PDK-10b981?style=flat-square&logo=circuitverse&logoColor=white" alt="PDK" />
  </p>

  <!-- Contact & Socials -->
  <p align="center">
    <a href="mailto:nguyentiendung12022006.vn@gmail.com" target="_blank">
      <img src="https://img.shields.io/badge/Email-nguyentiendung12022006.vn%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
    </a>
    &nbsp;
    <a href="https://github.com/vn-ntd" target="_blank">
      <img src="https://img.shields.io/badge/GitHub-vn--ntd-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
    </a>
    &nbsp;
    <a href="https://facebook.com/dung.12.02.2006" target="_blank">
      <img src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white" alt="Facebook" />
    </a>
  </p>

</div>

---

### 👨‍💻 Giới thiệu (About Me)

Kỹ sư định hướng chuyên sâu vào **ASIC / IC Physical Design (Backend)** và quy trình hiện thực hóa vi mạch số từ mã nguồn RTL đến layout chế tạo silicon (**RTL-to-GDSII**).

* 🔬 **Quy trình Physical Design (RTL-to-GDSII)**: Thực thi trọn vẹn luồng thiết kế vật lý bao gồm: Floorplanning, Power Planning (PDN), Standard Cell Placement, Clock Tree Synthesis (CTS), Routing và Post-route Optimization.
* ⏱️ **Timing Closure & STA**: Thành thạo phân tích Static Timing Analysis (STA), kiểm soát đường trễ Setup/Hold, giải quyết vi phạm timing thông qua **Timing ECO** (Buffer Insertion, Cell Sizing, Pin Swapping) và quản lý ràng buộc SDC.
* ⚡ **Toàn vẹn nguồn & Vật lý (Power & Reliability)**: Xây dựng lưới phân phối nguồn (Power Ring / Stripes), phân tích sụt áp **IR-Drop**, kiểm soát điện di động (EM) và tối ưu hóa diện tích / công suất (PPA).
* 🛡️ **Kiểm tra vật lý (Physical Signoff)**: Đảm bảo thiết kế đạt chuẩn chế tạo với **100% Clean DRC & LVS**, kiểm tra Antenna rules và trích xuất tham số ký sinh (Parasitic Extraction) trên tiến trình **SkyWater 130nm PDK**.
* ⚙️ **EDA Scripting & Automation**: Thành thạo lập trình kịch bản **Tcl**, **Python** và **Bash** để tự động hóa quy trình EDA, phân tích log và trích xuất chỉ số chất lượng thiết kế (QoR / PPA).

---

### 🔄 Quy trình Triển khai ASIC Backend (RTL-to-GDSII Flow)

```mermaid
flowchart LR
    A["RTL Design\n(Verilog / SV)"] --> B["Logic Synthesis\n(Yosys / SDC)"]
    B --> C["Floorplanning\n& PDN Design"]
    C --> D["Standard Cell\nPlacement"]
    D --> E["Clock Tree\nSynthesis (CTS)"]
    E --> F["Routing\n(Global & Detailed)"]
    F --> G["STA & Timing\nECO Closure"]
    G --> H["Physical Signoff\n(DRC / LVS / Antenna)"]
    H --> I["Tapeout Signoff\n(GDSII)"]
```

> 📌 **Tóm tắt quy trình:**  
> `RTL Design` ➔ `Logic Synthesis` ➔ `Floorplan & PDN` ➔ `Placement & CTS` ➔ `Routing` ➔ `STA & ECO` ➔ `DRC/LVS Verification` ➔ `GDSII Signoff`

---

### 🎯 Năng lực Kỹ thuật Cốt lõi (Core Competencies)

| Phân nhóm chuyên môn | Nội dung kỹ thuật & Trọng tâm công việc | Công cụ & Môi trường |
| :--- | :--- | :--- |
| 📐 **Physical Design & Floorplanning** | Xác định kích thước Core/Die, tỷ lệ khung (Aspect Ratio), vị trí Pin I/O, Macro Placement, Blockage/Halos, xây dựng lưới nguồn Power Distribution Network (PDN Rings & Stripes). | `OpenLane` `OpenROAD` `Magic VLSI` |
| 🚀 **Placement & Clock Tree Synthesis (CTS)** | Global & Detailed Placement, tối ưu hóa mật độ cell (Cell Density), giải tỏa nghẽn dây (Congestion), cấu trúc cây xung nhịp (Clock Inverter/Buffer Trees), cân bằng Clock Skew và hạn chế Insertion Delay. | `OpenROAD` `TritonCTS` |
| 🛣️ **Routing & DRC Closure** | Global Routing (FastRoute), Detailed Routing (TritonRoute), gán lớp kim loại (Layer Assignment), sửa lỗi Design Rule Check (DRC) và bảo vệ chân cổng tránh lỗi Antenna. | `TritonRoute` `KLayout` `Magic` |
| ⏱️ **Static Timing Analysis (STA) & ECO** | Khai báo ràng buộc thời gian (SDC), phân tích các góc hoạt động (PVT Corners), đóng vi phạm thời gian Setup/Hold bằng phương pháp Timing ECO Closure (Cell Resizing, Buffer Insertion). | `OpenSTA` `Python Automation` |
| 🔍 **Physical Verification & Signoff** | Kiểm tra quy tắc hình học (DRC), đối soát sơ đồ nguyên lý với layout (LVS), kiểm tra lỗi điện (ERC), trích xuất ký sinh SPEF (Parasitic Extraction) và xuất file GDSII chuẩn tapeout. | `Magic VLSI` `Netgen` `KLayout` |
| 🤖 **EDA Scripting & Automation** | Xây dựng script tự động hóa luồng chạy từ RTL đến GDSII, trích xuất dữ liệu timing/area từ log file, tự động hóa quy trình phân tích và báo cáo chất lượng PPA. | `Tcl / Tk` `Python` `Bash / Shell` `Linux` |

---

### 🛠️ Kỹ năng & Công cụ (Technical Stack)

#### 🔌 ASIC Physical Design & Backend
<p>
  <img src="https://img.shields.io/badge/Physical_Design-RTL_to_GDSII-0284c7?style=flat-square&logo=microchip&logoColor=white" alt="RTL to GDSII" />
  <img src="https://img.shields.io/badge/Floorplanning-Power_Planning_(PDN)-4f46e5?style=flat-square" alt="Floorplan & PDN" />
  <img src="https://img.shields.io/badge/CTS-Clock_Tree_Synthesis-7c3aed?style=flat-square" alt="CTS" />
  <img src="https://img.shields.io/badge/Routing-Global_&_Detailed-9333ea?style=flat-square" alt="Routing" />
  <img src="https://img.shields.io/badge/Timing_Closure-Setup%20%2F%20Hold%20ECO-c026d3?style=flat-square" alt="Timing ECO" />
  <img src="https://img.shields.io/badge/Physical_Signoff-DRC%20%2F%20LVS%20%2F%20Antenna-059669?style=flat-square" alt="DRC / LVS" />
</p>

#### ⚡ EDA Tools & PDKs
<p>
  <img src="https://img.shields.io/badge/SkyWater_130nm-PDK_Technology-00695C?style=flat-square&logo=circuitverse&logoColor=white" alt="SkyWater 130nm" />
  <img src="https://img.shields.io/badge/OpenLane-ASIC_Flow-0284c7?style=flat-square" alt="OpenLane" />
  <img src="https://img.shields.io/badge/OpenROAD-Physical_Design-2563eb?style=flat-square" alt="OpenROAD" />
  <img src="https://img.shields.io/badge/OpenSTA-Timing_Analysis-6b21a8?style=flat-square" alt="OpenSTA" />
  <img src="https://img.shields.io/badge/Yosys-Logic_Synthesis-ea580c?style=flat-square" alt="Yosys" />
  <img src="https://img.shields.io/badge/Magic_VLSI-DRC_&_Extraction-15803d?style=flat-square" alt="Magic" />
  <img src="https://img.shields.io/badge/Netgen-LVS_Signoff-047857?style=flat-square" alt="Netgen" />
  <img src="https://img.shields.io/badge/KLayout-GDSII_Viewer-0f766e?style=flat-square" alt="KLayout" />
</p>

#### 💻 Ngôn ngữ Lập trình & Scripting
<p>
  <img src="https://img.shields.io/badge/Tcl_/_Tk-EDA_Scripting-14b8a6?style=flat-square&logo=tcl&logoColor=white" alt="Tcl/Tk" />
  <img src="https://img.shields.io/badge/Python-Automation_&_Data-3b82f6?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Bash_/_Shell-Linux_Environment-4ade80?style=flat-square&logo=gnubash&logoColor=black" alt="Bash" />
  <img src="https://img.shields.io/badge/Verilog_HDL-Logic_Design-0284c7?style=flat-square&logo=c&logoColor=white" alt="Verilog" />
  <img src="https://img.shields.io/badge/SystemVerilog-Hardware_Verification-1d4ed8?style=flat-square" alt="SystemVerilog" />
  <img src="https://img.shields.io/badge/Linux_/_Unix-OS_Platform-f59e0b?style=flat-square&logo=linux&logoColor=black" alt="Linux" />
  <img src="https://img.shields.io/badge/Git-Version_Control-f97316?style=flat-square&logo=git&logoColor=white" alt="Git" />
</p>

---

### 🌟 Dự án IC Tiêu biểu (Featured IC Projects)

| Dự án | Mô tả Kỹ thuật & Kết quả Đạt được | Ngăn xếp Công nghệ |
| :--- | :--- | :--- |
| 🚀 [**`riscv_picorv32_sky130_asic_flow`**](https://github.com/vn-ntd/riscv_picorv32_sky130_asic_flow) | • Triển khai hoàn chỉnh luồng **RTL-to-GDSII** cho lõi vi xử lý **32-bit RISC-V (PicoRV32)**.<br/>• Đạt tần số hoạt động **133.3 MHz** với hệ số sử dụng diện tích lõi **Core Utilization ~70%**.<br/>• Đạt **100% Clean DRC, LVS & Antenna signoff** trên tiến trình **SkyWater 130nm PDK**. | `Verilog` `SkyWater 130nm` `OpenLane` `OpenROAD` `Magic` `Netgen` |
| ⏱️ [**`sta_timing_closure_eco`**](https://github.com/vn-ntd/sta_timing_closure_eco) | • Bộ công cụ và kịch bản phân tích Static Timing Analysis tự động hóa.<br/>• Tự động trích xuất slack vi phạm (Setup/Hold), đề xuất và thực hiện chèn buffer / cell sizing để đóng **Timing ECO Closure** hiệu quả. | `Python` `OpenSTA` `SDC Constraints` `EDA Automation` |
| ⚡ [**`pdn_analysis_ir_drop`**](https://github.com/vn-ntd/pdn_analysis_ir_drop) | • Mô phỏng và phân tích mạng lưới cấp nguồn (Power Distribution Network).<br/>• Đánh giá sụt áp tĩnh (Static IR-Drop), phát hiện các điểm nghẽn nguồn (hotspots) và tối ưu hóa mật độ thanh dẫn nguồn. | `Python` `PDN Modeling` `IR-Drop Analysis` |
| 🧰 [**`pd_flow_toolkit`**](https://github.com/vn-ntd/pd_flow_toolkit) | • Bộ công cụ script chuyên dụng cho kỹ sư Physical Design.<br/>• Tự động parse file log từ các công cụ EDA, trích xuất báo cáo chất lượng PPA (Power, Performance, Area) và tạo biểu đồ trực quan. | `Tcl` `Python` `Bash` `CI/CD for EDA` |

---

### 📊 Thống kê Hoạt động (GitHub Analytics)

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=vn-ntd&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117" height="150" alt="GitHub Stats" />
  &nbsp;
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=vn-ntd&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117" height="150" alt="Top Languages" />
</div>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=vn-ntd&theme=tokyonight&hide_border=true&background=0d1117" alt="GitHub Streak" />
</p>

---

<div align="center">
  💡 <i>"From RTL Architecture to Silicon Signoff — Engineering Resilient, High-Performance Physical Design Solutions."</i>
  <br/><br/>
  <sub>© 2026 <b>Nguyen Tien Dung (vn-ntd)</b> • IC Physical Design</sub>
</div>
