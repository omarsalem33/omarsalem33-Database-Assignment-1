# DriveNow - Database Design: ERD & Mapping

- **Name:** Omar Salem
- **Group:** `group 3`

Simulation Academy - .NET Diploma Cycle 1. Submission file: `DriveNow.drawio` (everything is inside it).

| draw.io page                 | Part | Content                                                                                                         |
| ---------------------------- | ---- | --------------------------------------------------------------------------------------------------------------- |
| 1-ERD-1-Staff-Training       | A    | BRANCH, EMPLOYEE (+ RENTAL_AGENT / MECHANIC specialization, SUPERVISES recursive 1:N), COURSE, TRAINING_ATTEMPT |
| 1-ERD-2-Fleet-Pricing        | A    | CATEGORY, CAR_MODEL, VEHICLE, rates (temporal), GPS_DEVICE (1:1), VEHICLE_TRANSFER                              |
| 1-ERD-3-Customers-Loyalty    | A    | CUSTOMER specialization, corporate drivers, discounts, blacklist, loyalty                                       |
| 1-ERD-4-Reservations-Rentals | A    | RESERVATION, RENTAL (1:1 reservation, 1:1 recursive EXTENDS), PROMO_CODE                                        |
| 1-ERD-5-Rental-Details       | A    | Extras, insurance (M:N), additional drivers, damage, violations, feedback                                       |
| 1-ERD-6-Maintenance-Payments | A    | Job cards, parts, suppliers (M:N), payments, invoices                                                           |
| 2-Schema-1 ... 2-Schema-4    | B    | 44 relational tables with PK / FK / NN / NULL / UQ / DF / CK                                                    |
| 3-Questions-Assumptions      | C    | 11 questions, 14 assumptions, 6 contradictions                                                                  |
| 4-Business-Rules             | D    | 8 rules that need triggers / procedures / application logic                                                     |

The ERD is split into 6 pages (max 10 entity boxes per page, dashed boxes for entities drawn elsewhere).

## Rebuild / export

```
python tools/build_drawio.py          # regenerates DriveNow.drawio (edit name/group/ID in tools/drawlib.py first)
python tools/export_pngs.py           # needs draw.io desktop; writes exports/<page-name>.png (zoom 100%, border 20, white, grid off)
```
