GUAM FAMILY TRAVEL MAP — pinch drift fix

- Pinch midpoint movement is separated from the original geographic anchor.
- The same map world contains both tiles and store pins.
- On pinch end, the visual scale is snapped to the committed integer zoom before recomputing center, preventing directional drift.
- New tile sets are layered over the old set so the map is not intentionally blanked during loading.
- Touch-action is disabled on the map so iPhone gestures remain inside the map.
