# airaware
AirAware 🌿 is a real-time environmental dashboard that provides air quality (AQI), PM2.5/PM10 levels, weather updates, UV index, and actionable health recommendations. Built for WeMakeDevs × AWS Environmental Hacks to promote smarter, healthier, and more environmentally aware living.

link - https://air-aware-environmental-safety-dashboard--bhuvanpno123.replit.app/

## 🏗️ System Architecture

AirAware uses AWS Lambda and API Gateway to retrieve live environmental data from Open-Meteo APIs.

```mermaid
flowchart TD
    A["User"] --> B["AirAware Web App"]
    B --> C["Amazon API Gateway"]
    C --> D["AWS Lambda"]
    D --> E["Open-Meteo Geocoding API"]
    D --> F["Open-Meteo Weather API"]
    D --> G["Open-Meteo Air Quality API"]
    E --> D
    F --> D
    G --> D
    D --> C
    C --> B
    B --> H["AQI Dashboard and Health Recommendations"]
```
