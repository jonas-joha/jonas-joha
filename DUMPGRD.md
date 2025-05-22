| S-4   | B-412; B-446                       | Dumping ground                                   | Point          |
|-------|-----------------------------------|-------------------------------------------------|----------------|
| S-57  | [11.4 Dumping ground (DMPGRD) P/A](#) |                                                 |                |
| Kort/ INT1 | N 23:1-2; N 62:1-2             |                                                 | Surface        |
| Real World |                               | GST Paper Chart                                  | ECDIS          |

Dumping ground is a sea area where dredged material or other potentially more harmful material, e.g. explosives, chemical waste, is deliberately deposited.

| Attribute                   | Allowable Encoding Value                                                                                  | Type | Multiplicity |
|-----------------------------|-----------------------------------------------------------------------------------------------------------|------|--------------|
| category of dumping ground (CATDPG) | 2 : chemical waste dumping ground<br>3 : nuclear waste dumping ground<br>4 : explosives dumping ground<br>5 : spoil ground<br>6 : vessel dumping ground | EN   | 0..*         |
| date discussed              |                                                                                                           | TD   | 0..1         |
| feature name                | See clause 2.5.8                                                                                           | C    | 0..*         |
| display mean language       | ISO 639-2/T                                                                                               | (S) BCTE | 0..1         |
| name usage                  | 1 : default name display<br>2 : alternate name display<br>3 : no chart display                             | (S) BEEN | 0..*         |
| restriction (RESTRN)        | 1 : anchoring prohibited<br>2 : anchoring restricted<br>3 : fishing prohibited<br>4 : fishing restricted<br>5 : trawling prohibited<br>6 : trawling restricted<br>7 : entry prohibited<br>8 : entry restricted<br>9 : dredging prohibited<br>10 : dredging restricted<br>11 : diving prohibited<br>12 : diving restricted<br>13 : no wakes<br>17 : discharging restricted<br>18 : industrial or mineral exploration/development prohibited<br>19 : industrial or mineral exploration/development restricted<br>20 : drilling prohibited<br>21 : drilling restricted<br>22 : removal of historical artefacts prohibited<br>23 : cargo transshipment (lightening) prohibited<br>24 : dragging prohibited<br>25 : stopping prohibited<br>27 : speed restricted | EN   | 0..*         |
| status (STATUS)             | 1 : permanent<br>2 : occasional<br>4 : not in use<br>6 : reserved<br>7 : temporary                           | EN   | 0..*         |
| scale minimum (SCAMIN)      | See clause 2.5.9                                                                                           | IN   | 0..1         |
| information                 | See clause 2.4.6                                                                                           | C    | 0..*         |
| file locator                |                                                                                                           | (S) TE | 0..1         |
| file reference              |                                                                                                           | (S) TE | 0..1         |
| headline                   |                                                                                                           | (S) TE | 0..1         |
| language                   | ISO 639-2/T                                                                                               | (S) TE | 0..1         |
| text                       |                                                                                                           | (S) TE | 0..*         |

**Additional Information**

- ArcMap Menu: RegulatedAreaAndLimits\DMPGRD_DumpingGround  
- Encoding Instructions: RegulatedAreaAndLimits\DMPGRD_DumpingGround  

**Remarks**

Use the attribute INFORM to indicate the specified least depth (e.g.):

1. If specified depth given:  
   "In the Danish Environmental Protection Agency permit for dumping, it is stated that the dumping should not reduce the depth within the area to less than xx.x metres in relation to mean sea level (MSL)."

2. If no specified depth is not given:  
   "The Danish Environmental Protection Agency permit for dumping does not state a limiting depth to dumping within this area."

**Policy and references**  
[UOC 11.4 Dumping & Spoil grounds](https://wetp.wufoo.com/forms/uoc-114-dumping-spoil-grounds/)
