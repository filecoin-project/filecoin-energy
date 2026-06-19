# Model SQL Table References
You can find the model that generates each graph in the models folder.

| Index | Model Name | File | Tables in FROM Clauses |
|------:|------------|------|------------------------|
| 1 | Energy consumption rate (v1.0.2) | `010_total_energy-model-v-1-0-2.js` | `fil_miners_data_view_country_v9`, `fil_sealed_capacity_view_v2`, `fil_miners_location` |
| 2 | Energy used to seal data (v1.0.2) | `008_sealing_energy-model-v-1-0-2.js` | `fil_sealed_capacity_view_v2`, `fil_miners_location` |
| 3 | Energy used to store data (v1.0.2) | `009_storage_energy-model-v-1-0-2.js` | `fil_miners_data_view_country_v9` |
| 4 | Cumulative Energy Use (v1.0.2) | `016_cumulative-energy-use-model.js` | `fil_miners_data_view_country_v9` |
| 5 | Location-Based Emissions (Ignoring Renewable Energy Purchases) | `019_total-emissions-model.js` | `fil_miners_data_view_country_v9` |
| 6 | Market-Based Emissions (Including Renewable Energy Purchases) | `021_total-emissions-with-renewable-floor-model.js` | `fil_miners_data_view_country_v9` |
| 7 | Data storage capacity added per day | `003_sealed-model.js` | `fil_sealed_capacity_view_v2`, `fil_miners_location` |
| 8 | Data storage capacity | `001_capacity-model.js` | `fil_miners_data_view_country_v9` |
| 9 | Energy per transaction | `026_energy-per-transaction-model.js` | `fil_messages_stats` |
| 10 | Emissions per transaction | `027_emissions-per-transaction-model.js` | `fil_messages_stats` |
| 11 | Renewable Energy Share of Total Energy | `028_miners-energy-re-share-model.js` | `fil_miners_energy_re_share` |

## Distinct Tables

- `fil_miners_data_view_country_v9`
- `fil_miners_energy_re_share`
- `fil_miners_location`
- `fil_messages_stats`
- `fil_sealed_capacity_view_v2`

