# Open Climbing Center Dataset

An open, community-maintained dataset of indoor climbing and bouldering centers around the world.

The goal of this project is to provide a freely reusable, structured dataset containing factual information about climbing centers, including:

* Climbing center names
* Chain/operator (brand)
* Street addresses
* City, region, country, and continent
* Official homepage URLs
* GPS coordinates
* Available climbing disciplines and training boards

## Dataset Format

The primary dataset is stored as a single CSV file:

```text
climbing_centers.csv
```

Current schema:

| Column           | Description                                                |
| ---------------- | ---------------------------------------------------------- |
| `id`             | Stable unique identifier for the climbing center.          |
| `brand`          | Operating company or chain (e.g. Boulders, Beta Boulders). |
| `gym_name`       | Name of the physical climbing center.                      |
| `street_address` | Street address.                                            |
| `postal_code`    | Postal code.                                               |
| `city`           | City or municipality.                                      |
| `region`         | Region, state, or province (optional).                     |
| `country`        | Country name.                                              |
| `homepage`       | Official website of the center or chain.                   |
| `latitude`       | Latitude in decimal degrees (optional).                    |
| `longitude`      | Longitude in decimal degrees (optional).                   |
| `bouldering`     | `true` if bouldering is available.                         |
| `lead`           | `true` if lead climbing is available.                      |
| `top_rope`       | `true` if top rope climbing is available.                  |
| `moonboard`      | `true` if a MoonBoard is available.                        |
| `kilterboard`    | `true` if a Kilter Board is available.                     |
| `spraywall`      | `true` if a spray wall is available.                       |
| `continent`      | Continent name.                                            |

## Data Guidelines

* One row represents **one physical climbing center**.
* Chains with multiple locations should have one entry per location, sharing the same `brand`.
* Unknown values should be left blank rather than using `N/A` or `null`.
* Boolean fields should use lowercase `true` or `false`.
* The CSV file should be encoded as UTF-8 to preserve local characters.
* Latitude and longitude should use standard WGS84 decimal coordinates.

## Contributing

Contributions are welcome! You can help by:

* Adding missing climbing centers.
* Updating addresses or homepages.
* Adding GPS coordinates.
* Correcting facility information (lead, bouldering, MoonBoard, etc.).
* Expanding coverage to additional countries and continents.

Please verify information against official gym websites or other reliable public sources whenever possible.

## License

* **Code and scraping utilities:** MIT License.
* **Dataset:** CC0 1.0 Universal (Public Domain Dedication).

The dataset contains factual information intended to be freely reused by the climbing community for apps, research, maps, and other projects. Attribution is appreciated but not required.
