GUAM FAMILY TRAVEL MAP — pinch drift fix

- Pinch midpoint movement is separated from the original geographic anchor.
- The same map world contains both tiles and store pins.
- On pinch end, the visual scale is snapped to the committed integer zoom before recomputing center, preventing directional drift.
- New tile sets are layered over the old set so the map is not intentionally blanked during loading.
- Touch-action is disabled on the map so iPhone gestures remain inside the map.


【MAP表示修正】おすすめフィルター追加時に誤って未定義のrenderMarkers()を呼んでJavaScriptが停止していたため、renderMap()へ修正。LeafletはjsDelivr→cdnjsのフォールバックを追加し、初期化の二重実行も防止。
