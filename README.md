# wc-leaflet-map

## Installation

Bower dependency:
```
    "wc-leaflet-map": "https://github.com/seabourne/wc-leaflet-map.git"
```


## Usage

```
<link rel="import" href="../../../bower_components/wc-leaflet-map/leaflet-map.html">
<link rel="import" href="../../../bower_components/wc-leaflet-map/leaflet-marker.html">
<link rel="import" href="../../../bower_components/wc-leaflet-map/leaflet-cluster-group.html">
<link rel="import" href="../../../bower_components/wc-leaflet-map/leaflet-controls.html">

```

Defines the following components:


### leaflet-map

```
  <leaflet-map map="{{map}}"
               tile-layer="mapbox.streets"
               zoom-level="10"
               starting-lat-lon="[23, 78.05]"
               options="{L.mapbox.map options}"
               ></leaflet-map>
```

### leaflet-marker

```
  <template is="dom-bind">
    <leaflet-map map="{{map}}">
      <leaflet-marker map="{{map}}" location="[23, 78.05]" options="{L.marker options}">
        <p>Contents</p>
      </leaflet-marker>
    </leaflet-map>
  </template>
```

### leaflet-cluster-group

```
  <template is="dom-bind">
    <leaflet-map map="{{map}}">
      <leaflet-cluster-group map="{{map}}" markers="{{markers}}">
        <leaflet-marker map="{{markers}}" location="[23, 78.05]" options="{L.marker options}">
          <p>Contents</p>
        </leaflet-marker>
      </leaflet-cluster-group>
    </leaflet-map>
  </template>
```


### leaflet-controls

```
  <template is="dom-bind">
    <leaflet-map map="{{map}}">
      <leaflet-controls map="{{map}}" feature-group="{{featureGroup}}" geo="{{geo}}" draw-options="{L.Control.Draw draw options}">
      </leaflet-controls>
    </leaflet-map>
  </template>
```
