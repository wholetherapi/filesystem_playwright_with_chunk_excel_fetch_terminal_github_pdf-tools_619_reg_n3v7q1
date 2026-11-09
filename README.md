# Ravensworth Instrumentation Consortium — Certification Records

Public certification registry maintained by the consortium programme office.

`records.json` holds one record per certified track. A record has the following
fields:

| Field | Meaning |
| --- | --- |
| `track_id` | Track identifier (for example `RE-PD-04`) |
| `track_name` | Human-readable track name |
| `division` | Division that processes the submission |
| `status` | `certified` once the submission is complete |
| `minimum_field_validation_hours` | Integer requirement for the track |
| `source_url` | Link to the first-party page that states the requirement |
| `implementation` | Object with `package`, `spec_id` and `monthly_downloads` |
| `excluded_candidates` | Array of objects with `package` and `reason` |
| `updated_at` | Date the record was last updated |

Records are append-only per track: update the existing record for a track rather
than duplicating it, and keep other tracks untouched.
