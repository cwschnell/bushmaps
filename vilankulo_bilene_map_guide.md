# Vilankulo to Bilene Bush Roads Map Guide

This guide explains how to use the map and how to extend a saved red road line with OSRM.

## Open the map

1. Open `vilankulo_chibuene_pomene_map.html` in a web browser.
2. Wait for the satellite map to load.
3. Zoom in close when looking for small bush roads.
4. Use the layers button in the top right to switch between satellite, OpenStreetMap, and the R road layer.

## What the map colours mean

- Red line: your saved road line.
- Green marker: the current end of the red line when OSRM extension mode is on.
- Orange marker: correction point used for trimming part of a red line.
- Blue line: temporary OSRM route before it is saved.
- Blue markers: start and current end of the temporary blue OSRM route.
- R layer lines: roads or tracks already mapped in OpenStreetMap.

Move the mouse over lines and markers on the map to see explanations.

## Extend a red saved road with OSRM

1. Click the red line once to select it.
2. Click `Continue selected as OSRM`.
3. The button must change to `OSRM extension ON - click next point`.
4. Look for the green marker. This is where the red line will continue from.
5. Click a point farther along the road, not on the green marker itself.
6. If OSRM finds a mapped road, the red line extends to that point.
7. The green marker moves to the new end.
8. Click the next point farther along the road.
9. Repeat this step by step until the road is long enough.
10. Click the OSRM extension button again when finished.

## If OSRM does not draw the next section

OSRM can only follow roads that are already mapped in OpenStreetMap.

If the satellite image shows a bush track but OpenStreetMap does not know about that track, OSRM cannot draw it. In that case, use manual drawing:

1. Click `Start drawing`.
2. Click short points along the visible bush road.
3. Click every bend or change of direction.
4. Click `Finish line` when done.

## Correct part of a red line

1. Click the red line near the place where the correction must start.
2. An orange correction point appears.
3. Click `Trim after pointer` to remove the red line after that orange point.
4. Click `Trim before pointer` to remove the red line before that orange point.
5. Click `Continue selected as OSRM` to rebuild from the new end, or use manual drawing if the bush road is not mapped in OpenStreetMap.

## Undo

Click `Undo previous action` to undo the last map change. It works for blue route clicks, clearing the blue route, saving, importing, deleting, trimming, joining, OSRM extension, following OSM road, saving a blue OSRM route, and clearing the map.

## Clear the blue route

Click `Clear blue route` to remove the temporary blue route and its blue pins. If you clicked it by mistake, click `Undo previous action`.

## Clear the map

Click `Clear map` to remove all red saved roads and the temporary blue route from the screen. If you clicked it by mistake, click `Undo previous action` to restore the previous map.

## Save or share your work

- Use `Export saved lines` to save your red road lines as GeoJSON.
- Use `Import lines` to load a saved GeoJSON file again.
- Click a red line to see its start and end markers. The white dot is the start, and the red dot is the end.
- Use `Join selected + nearest` to join one selected red section to the closest other red section.
- Use `Join red lines` after importing or saving several road stretches. This creates one new joined red road and keeps the original pieces.
- If the joined road shows a straight connector, there is a gap between the saved sections. Trim the bad part and redraw the missing piece before exporting.
- Click the joined red road, then use `Export Google Maps line` to save a KML file.
- To view the KML in Google Maps, open Google My Maps in a browser, create a map, choose Import, and select the KML file.
- The shareable zip file is `vilankulo_to_bilene_bush_roads_map.zip`.
