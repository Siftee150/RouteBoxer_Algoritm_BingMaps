# RouteBoxer_Algoritm_BingMaps
Implementation of RouteBoxer Algorithm,originally done using Google Maps Api,done using Bing maps Api.
The implementation is,right now,limited in its features as it only generates route boxes for the route already generated by Bing Maps Direction Service and not
for a path of polylines etc.
In order to use the routeboxer function, type in the following command in the javascript project you wish to use it on:

var currentRoute = directionsManager.getCurrentRoute(); (directionsManager is just a name, you can give any name to this directionManager class instance)
var box = RouteBoxer.box(currentRoute.routePath,distance);

Here the currentRoute.routePath is the route as generated by Bing Maps Direction Service,and is basically an array of locations forming the path.
Distance is specified in kilometers and specifies the range to the routeboxer algorithm so that it computes boxes accordingly.

The route boxer algorithm returns an array of BoundingBoxes(which are called LocationRect in Bing Maps) as a result. This is stored in the variable box 
in the above example.

Lastly,I am only a student who needed this implementation for a project. I shared it incase it helps. This is not an official implementation. 
