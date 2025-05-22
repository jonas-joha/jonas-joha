## DM(DPGRD) – Dumping Ground   (**Point**, ~~Curve~~, **Surface**)

**S-4 references**: B-412; B-446  
**S-57 references**: 11.4 Dumping ground (DM(DPGRD) P/A)  
**INT1**: N23.1-2  

> **Definition:**  
> A dumping ground is a sea area where dredged material or other potentially more harmful material (e.g. explosives, chemical wastes) is deliberately deposited.

---

| Real World                       | GST Paper Chart                      | ECDIS                   |
|----------------------------------|--------------------------------------|-------------------------|
|                                  |![image-20221002-123102](https://github.com/user-attachments/assets/6ab4ab36-6402-4161-882b-1bcd030cd918) ![image-20221002-123117](https://github.com/user-attachments/assets/d33f5ff7-a611-4e8c-b006-83a7aa6a4fc0) |
---

## Attribute Encoding Table

| Attribute                        | Code(s)                    | Allowed Encoding Values / Format                                                                                                                                                                                                                                                                                                                                                         | Type | Multiplicity |
|----------------------------------|----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|--------------|
| **Category of dumping ground**   | `CATDPG`                   | `2` – Chemical waste dumping ground<br>`3` – Nuclear waste dumping ground<br>`4` – Explosives dumping ground<br>`5` – Spoil ground<br>`6` – Vessel dumping ground                                                                                                                                                                                                                       | EN   | 0..*         |
| **Date discussed**               | `dateDiscussed`            | [ISO 8601 date]                                                                                                                                                                                                                                                                                                                                                                         | TD   | 0..1         |
| **Feature name**                 | `featureName`              | See clause 2.5.8                                                                                                                                                                                                                                                                                                                                                                        | C    | 0..*         |
| **Display encoding language**    | `dgnEncodingLanguage`      | ISO 639-2/T                                                                                                                                                                                                                                                                                                                                                                             | S    | 1..1         |
| **Name usage**                   | `OBJNAM` / `NOBJNAM`       | `1` – Default name display<br>`2` – Alternate name display<br>`3` – No chart display                                                                                                                                                                                                                                                                                                    | EN   | 0..1         |
| **Restriction**                  | `RESTRN`                   | `1` – Anchoring prohibited<br>`2` – Anchoring restricted<br>`3` – Fishing prohibited<br>`4` – Fishing restricted<br>`5` – Trawling prohibited<br>`6` – Trawling restricted<br>`7` – Entry prohibited<br>`8` – Entry restricted<br>`9` – Dredging prohibited<br>`10` – Dredging restricted<br>`11` – Diving prohibited<br>`12` – Diving restricted<br>`13` – No wake<br>`17` – Discharging restricted<br>`18` – Industrial/mineral exploration/development prohibited<br>`19` – Industrial/mineral exploration/development restricted<br>`20` – Drilling prohibited<br>`21` – Drilling restricted<br>`22` – Removal of historical artefacts prohibited<br>`23` – Cargo transhipment (lightering) prohibited<br>`24` – Dragging prohibited<br>`25` – Sloping prohibited<br>`27` – Speed restricted | EN   | 0..*         |
| **Status**                       | `STATUS`                   | `1` – Permanent<br>`2` – Occasional<br>`4` – Not in use<br>`5` – Reserved<br>`7` – Temporary                                                                                                                                                                                                                                                                                            | EN   | 0..*         |
| **Minimum display scale**        | `SCAMIN`                   | See clause 2.5.9                                                                                                                                                                                                                                                                                                                                                                        | IN   | 0..1         |
| **Information**                  | `INFORM`                   | See clause 2.5.6                                                                                                                                                                                                                                                                                                                                                                        | C    | 0..*         |
| **File locator**                 | `FTXLOC` / `NTXLOC`        | Free text (e.g. URL or path)                                                                                                                                                                                                                                                                                                                                                            | TE   | 0..1         |
| **File reference**               | `FTXTDSC` / `NTXTDSC`      | Free text (e.g. document title)                                                                                                                                                                                                                                                                                                                                                          | TE   | 0..1         |
| **Headline**                     | `HEADLN`                   | Free text                                                                                                                                                                                                                                                                                                                                                                               | TE   | 0..1         |
| **Language**                     | `LANG`                     | ISO 639-2/T                                                                                                                                                                                                                                                                                                                                                                             | TE   | 1..1         |
| **Text**                         | `INFORM` (multi-line)      | Free text content                                                                                                                                                                                                                                                                                                                                                                       | C    | 0..*         |

---

## Additional Information

- **ArcMap menu path:**  
  `RegulatedAreasAndLimits\DM(DPGRD)_DumpingGround`

- **Encoding instructions:**  
  RegulatedAreasAndLimits\DM(DPGRD)_DumpingGround

- **Compilation instructions:**  
  _(none)_

- **Scale:**  
 Charts shall follow the standard IHO 1-2-5 progression (… 1:5 000; 1:10 000; 1:20 000; 1:50 000; 1:100 000; 1:200 000; 1:500 000; 1:1 000 000…).<br><br>Dumping grounds (S-4 B-412/B-446) are to be shown at scales equal to or larger than the dataset’s compilation scale (e.g. coastal, approach and harbour scales) and may be suppressed at smaller scales via the `SCAMIN` attribute.

- **Remarks:**  
  1. Use the `INFORM` attribute to record the specified least depth (m).  
  2. **If a depth is specified**, e.g.:  
     > “The Danish Environmental Protection Agency permit for dumping is given; it is stated that the dumping should not reduce the depth within the area to less than x.x metres in relation to mean sea level (MSL).”  
  3. **If no depth is specified**, e.g.:  
     > “The Danish Environmental Protection Agency permit for dumping does not state a limiting depth to dumping within this area.”

---

## References

- **IHO S-4:** B-412; B-446  
- **IHO S-57:** Clause 11.4 (DM(DPGRD) P/A)
