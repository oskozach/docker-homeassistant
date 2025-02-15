# Docker | Home Assistant

This is a Home Assistant setup running in Docker, supporting Node-RED custom component and eWeLink Smart Home, TasmoAdmin addons.

## Node Red Custom Component
```
cd config && \
    mkdir custom_components && \
    cd custom_components && \
    git clone https://github.com/zachowj/hass-node-red.git && \
    mv hass-node-red/custom_components/nodered . && \
    rm -rf hass-node-red && \
    cd ../..
```
- Restart Home Assistant
- Settings > Devices & Services > Add integration > search Node-RED > Install

## eWeLink Addon
```
mkdir ./addons && \
    cd ./addons && \
    git clone https://github.com/CoolKit-Technologies/ha-addon.git && \
    mv ha-addon ewelink && \
    cd ..
```