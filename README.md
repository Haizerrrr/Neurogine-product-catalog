# Product Catalog App - Technical Assessment

Developed by: Haiza
Position: Junior Mobile Developer
Company: Neurogine

## Tech Stack & Architecture
- **Framework:** React Native (Expo)
- **API:** DummyJSON Products API
- **Architecture:** 2-Layer Pattern
  - **Data Layer:** API interaction handling pagination, search querying, and detail retrieval.
  - **Presentation Layer:** State-driven UI managing loading spinners, error fallback with retry logic, empty states, and dynamic catalog rendering.

## Search Strategy & Debounce
- Utilizes the DummyJSON server-side search endpoint (`/products/search?q=...`) combined with a 500ms debounce.
- **Decision rationale:** Server-side querying ensures accurate searches across the complete catalog dataset rather than restricting results to items already cached in memory.

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone [https://github.com/Haizerrrr/Neurogine-product-catalog.git](https://github.com/Haizerrrr/Neurogine-product-catalog.git)
   cd Neurogine-product-catalog
