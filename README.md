[![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/nfa-vfxim/tk-photoshopcc?include_prereleases)](https://github.com/nfa-vfxim/tk-photoshopcc) 
[![GitHub issues](https://img.shields.io/github/issues/nfa-vfxim/tk-photoshopcc)](https://github.com/nfa-vfxim/tk-photoshopcc/issues) 


# ShotGrid Engine for Photoshop CC <img src="icon_256.png" alt="Icon" height="24"/>

ShotGrid Integration for Photoshop CC

## Requirements

| ShotGrid version | Core version | Engine version |
|------------------|--------------|----------------|
| -                | v0.19.18     | -              |

**Frameworks:**

| Name                      | Version | Minimum version |
|---------------------------|---------|-----------------|
| tk-framework-shotgunutils | v5.x.x  |                 |
| tk-framework-adobe        | v1.x.x  |                 |



## Configuration

### Booleans

| Name                       | Description                                                         | Default value |
|----------------------------|---------------------------------------------------------------------|---------------|
| `automatic_context_switch` | Controls whether an active document change causes a context change. | True          |
| `debug_logging`            | Controls whether debug messages should be emitted to the logger     | False         |


### Lists

| Name              | Description                                                                                                                                                                                                                                                                                                                                             | Default value |
|-------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|
| `shelf_favorites` | Controls the registered commands that show up in the favorites shelf in the ShotGrid panel. This is a list where each item is a dictionary with keys 'app_instance' and 'name'. The 'app_instance' key connects this entry to a particular app instance defined in the environment configuration file. The 'name' is a command name to make a favorite. | []            |


### Hooks

| Name                          | Description                                                                             | Default value                    |
|-------------------------------|-----------------------------------------------------------------------------------------|----------------------------------|
| `context_fields_display_hook` | Hook which controls how context fields are queried and displayed in the context header. | {self}/context_fields_display.py |


