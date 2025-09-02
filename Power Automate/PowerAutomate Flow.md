⚡ **Power Automate flow description:**

- Trigger – The flow runs daily at 08:00 AM.

- Authentication – Request token from the API and parse JSON response.

- Initialize variables – Store token and prepare the request payload.

- Data request – Call the API to fetch valuation data.

- Storage – Save the raw JSON response into Tables.json for further processing in Power Query.

---
**Diagram:**

```mermaid
flowchart TD
    A[Daily Recurrence 08:00 AM] --> B[Request Token from Database API]
    B --> C[Parse JSON]
    C --> D[Initialize variable Token]
    D --> E[Initialize variable Request Message JSON]
    E --> F[Request Asset Valuation JSON]
    F --> G[Create file Tables.json]
```