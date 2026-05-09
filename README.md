# IoT-Data-Simulation-Group6

The project simulates various data points typically collected by IoT devices in a logistics environment, such as GPS locations, environmental sensors (temperature), and vehicle telematics.

## Features
* **Data Generation**: Simulates 100 unique shipment records with diverse attributes.
* **IoT Parameters**: Includes simulated data for RFID tags, vehicle IDs, driver IDs, and real-time status tracking (`In Transit`, `Delivered`, `Delayed`, `Cancelled`).
* **Environmental Monitoring**: Generates temperature data (Celsius) to simulate cold-chain or sensitive cargo monitoring.
* **Operational Metrics**: Calculates cargo weight, fuel consumption, average speed, transport costs, and CO2 emissions.
* **Delay Analysis**: Automatically calculates `delay_hours` by comparing scheduled delivery times against actual delivery times.
* **Multi-format Export**: Supports exporting the generated dataset to both `.csv` and `.json` formats for integration with other analytics tools.

## Key Data Fields
The simulation generates the following fields for each record:
* **Identifiers**: `timestamp`, `shipment_id`, `rfid_tag`, `vehicle_id`, `driver_id`
* **Route**: `origin`, `destination` (Includes hubs like Manila, Cebu, Davao, Clark, and Iloilo), `distance_km`
* **Logistics**: `scheduled_delivery`, `actual_delivery`, `status`, `delay_hours`
* **Cargo**: `cargo_weight_kg`, `cargo_type` (Electronics, Food, Clothing, Furniture, Pharmaceuticals)
* **Metrics**: `fuel_consumed_l`, `avg_speed_kmh`, `temperature_c`, `transport_cost_usd` / `transport_cost_php`, `co2_emissions_kg`

## Usage
1. Open the `MO-IT148 Homework IoT Data Simulation H3101 Group Six.ipynb` notebook.
2. Run the cells sequentially.
3. The script will generate a new set of randomized records and automatically save them as `logistics_data.csv` and `logistics_data.json` in your local directory.
