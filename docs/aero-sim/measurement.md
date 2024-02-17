# Measurement

| Property| Type| Description|
|------------------|--------|-------------------------------------------------------|
| Gases| Map<GasType, AtmosphericGas> | Holds the list of gases used.|
| Is Toxic| Boolean| If true, at least one gas has a toxicity level above 0.|
| Humidity| Float| Current humidity level.|
| Temperature| Float| Current temperature level.|
| Pressure| Float| Current pressure level.|

## Atmospheric Gas

| Property| Type| Description|
|------------------|--------|-------------------------------------------------------|
| Name| String| Name of the target gas.|
| Config | Gas Config| Gas properties. |
| Molecular Weight| Float| Molecular weight of the gas.|
| Density| Float| Density of the gas.|
| Color| Color| Color used for visual representation of the gas.|
| Toxicity| Float| Toxicity level of the gas, ranging from non-toxic (0) to very toxic (1). |
| Boiling Point| Float| Boiling point of the gas in Celsius.|

### Gas Config

| Property| Type| Description|
|-------------------|-----------|--------------------------------------------------------------------|
| Concentration| Float| The concentration/level/amount of the gas. {==What this value represents in your game is up to you.==}|
| Gas Emission| Float| The rate at which gas is emitted. {==Ignored by Absorbers==}|
| Gas Absorption| Float| The rate at which gas is absorbed. {==Ignored by Vents==}|
| Max Gas Increase| Float| Maximum increase limit for gas concentration. {==Ignored by Absorbers==}|
| Max Gas Decrease| Float| Maximum decrease limit for gas concentration. {==Ignored by Vents==}|
