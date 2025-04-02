# Grid-Operations-Dashboard
**Comprehensive Grid Analytics for Utility Operations**  

---

## Project Overview  
This interactive dashboard suite provides end-to-end visibility into power distribution performance across **circles, districts, and feeders**. It combines auto-recloser analytics, voltage monitoring, and operational trends to optimize grid reliability and maintenance planning.  

---

## Dashboard Modules  

### 1. Auto Recloser Dashboard  
   - **Function**: Tracks auto-recloser operations (lockout vs. operated events).  
   - **Key Metrics**:  
     - Success/failure rates by feeder (e.g., Bawana: $14 cost impact).  
     - Hierarchical filters (Circle → District → Zone).  
   - **Insight**: Prioritize feeders with high lockout rates (e.g., Narela, Kirari).  

### 2. Power Distribution Dashboard  
   - **Function**: Monitors 11 kV line performance and financial impact.  
   - **Key Metrics**:  
     - **43% success rate** (101 operations).  
     - Annual trends (FY 2019–2025).  
     - Hotspot zones (Sub-Urban Circle: 507/514 operations).  
   - **Insight**: Low success rates indicate need for equipment calibration.  

### 3. Circle Operations Overview  
   - **Function**: Aggregates fault data by geographical hierarchy.  
   - **Key Metrics**:  
     - **District-level totals** (e.g., Urban Circle: Bawana-439, Narela-431).  
     - Feeder-specific events (e.g., "MBS Bawana 5/8 (O/D)").  
   - **Insight**: Urban Circle contributes 63% of total faults (focus area).  

---

## Key Features  

### Interactive Controls  
- **Dynamic Filters**:  
  - Time range (FY selection).  
  - Geographical drill-down (Circle → District → Feeder).  
- **Comparative Analysis**:  
  - Lockout vs. operated events.  
  - Year-over-year performance.  

### Data Visualizations  
- **Tabular Reports**: District-wise fault counts (e.g., Metro vs. Sub-Urban).  
- **Geographical Heatmaps**: Fault density by feeder (if available).  
- **Trend Charts**: Monthly outage patterns.  

---

## Dataset & Methodology  
- **Sources**: SCADA, outage logs, financial records.  
- **Cleaning**:  
  - Standardized feeder names (e.g., "BAVIANA" → "Bawana").  
  - Removed incomplete entries (e.g., null voltage readings).  
- **Calculations**:  
  - Success % = (Operated Events / Total Operations) × 100.  
  - Cost impact = Sum of repair costs per feeder.  

---

## Insights & Recommendations  
- **Critical Feeders**: Bawana (439 faults) and Narela (431 faults) need infrastructure upgrades.  
- **Recloser Optimization**: Low success rates (43%) suggest recalibration or replacement.  
- **Resource Allocation**: Focus on Urban Circle (highest fault volume).  

---

## How to Use  
1. **Navigation**:  
   - Use dropdowns to filter by FY, circle, or feeder.  
   - Click on a feeder in maps/tables to view detailed logs.  
2. **Export**: Generate PDF/Excel reports for audits.  

---

## Future Enhancements  
- **Predictive Analytics**: Fault forecasting using weather/data trends.  
- **Mobile Alerts**: Real-time notifications for lockout events.  

---

## Glossary  
| Term | Definition |  
|------|------------|  
| **Lockout** | Auto-recloser failed to restore power (manual reset required) |  
| **Operated** | Successful auto-reclose operation |  
| **0BADU** | Feeder ID (e.g., Bawana feeder) |  
| **FY** | Financial Year (April-March cycle) |  
