## Hi there 👋

## Open Source Contributions

### WebGL & Map Tiles

- **[Martin](https://github.com/maplibre/martin)** · [#3569](https://github.com/maplibre/martin/pull/3569)
  Enabled PGO for ARM64 and PGO + BOLT for x86_64 binaries used by base Linux Docker images in nightly and release builds. Across four PostGIS fixture scenarios, measured median throughput gains of 3.8–5.4% on ARM64 and 2.6–7.4% on x86_64.

- **[MapLibre GL JS](https://github.com/maplibre/maplibre-gl-js)** · [#8715](https://github.com/maplibre/maplibre-gl-js/pull/8715)
  Fixed a rendering crash triggered by removing a feature-state property before any state exists. Added a guard in `SourceFeatureState.coalesceChanges()` and a focused regression test for the missing-state case.

- **[luma.gl](https://github.com/visgl/luma.gl)** · [#3429](https://github.com/visgl/luma.gl/pull/3429)
  Added guards that reject buffer, texture, shader, and sampler creation when the WebGL context is already lost, before unusable resources are registered. Added a regression test using real context loss to verify clear errors and unchanged active-resource counts.

### Spring

- **[Spring Framework](https://github.com/spring-projects/spring-framework)** · [#36830](https://github.com/spring-projects/spring-framework/pull/36830)
  Contributed `String`-to-`DataSize` and `Number`-to-`DataSize` converters to `DefaultConversionService`, making these conversions available through Spring Framework's default conversion service. Added tests for parsing, empty strings, and invalid inputs.

- **[Spring Data Relational](https://github.com/spring-projects/spring-data-relational)** · [#2299](https://github.com/spring-projects/spring-data-relational/pull/2299)
  Contributed bidirectional conversion between H2 `Interval` and Java `Duration`, with tests for day-time intervals, negative durations, and database round trips. The maintainer adapted the implementation for both JDBC and R2DBC before merging.

### Kubernetes & Terraform

- **[terraform-provider-harbor](https://github.com/goharbor/terraform-provider-harbor)** · [#606](https://github.com/goharbor/terraform-provider-harbor/pull/606)
  Added `oidc_client_secret_wo` and a version-based secret update trigger to `harbor_config_auth`. Included configuration validation, usage documentation, and tests covering secret handling, rotation, and exclusion of the write-only secret from Terraform state.

- **[valkey-operator](https://github.com/valkey-io/valkey-operator)** · [#190](https://github.com/valkey-io/valkey-operator/pull/190)
  Removed the `-config` suffix from default operator-managed ConfigMap names, changing `valkey-<name>-config` to `valkey-<name>`. Updated the naming test and corrected the end-to-end cleanup check to use the controller's naming helper.

### AI Coding Tools

- **[BMAD-METHOD](https://github.com/bmad-code-org/BMAD-METHOD)** · [#2386](https://github.com/bmad-code-org/BMAD-METHOD/pull/2386)
  Added Korean documentation, a Korean README, translated workflow diagrams, and localized navigation and Starlight UI strings. Registered the Korean website locale and synchronized the translations with upstream documentation changes throughout the PR.
