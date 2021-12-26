# TrackBuilder
Building train tracks for the IKEA Lilleby system.

Initially, an algorthm to build valid layouts (i.e. layouts without tracks ending with missing connections), out of IKEA Lilleby train tracks.

Valid track:
- closed track: no missing connections, no track has an unconnected endpoint (this changes if we introduce dead-end stop points)
- within borders: no part outside of the assigned floor area
- within height limits: no parts above maximum height nor below floor level
- within track limits: not using more tracks than are physically available (the user can set how many pieces of each type is available)
- no crossings: no tracks on top of others, unless it is on different levels

Next, maybe use a neural network AI to make the algorithm smarter, i.e. able to create valid and high-quality tracks as quickly as possible 

Quickly: mis-placing as few tracks as possible

High-quality: 
- using many track pieces
- some straight parts
- some long curves
- some bridge crossings
- some switches
- long sections between switches
- using the full area, getting close but not too close, to the edges
