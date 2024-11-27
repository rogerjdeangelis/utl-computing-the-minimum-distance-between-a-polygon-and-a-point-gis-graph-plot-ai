# utl-computing-the-minimum-distance-between-a-polygon-and-a-point-gis-graph-plot-ai
Computing the minimum distance between a polygon and a point gis graph plot ai
    %let pgm=utl-computing-the-minimum-distance-between-a-polygon-and-a-point-gis-graph-plot-ai;

    %stop_submission;

    Computing the minimum distance between a polygon and a point gis graph plot ai

    SOAPBOX ON

    Python is a better choice for image processing than R.
    Consider OpenCV, premier face detection software.

    SOAPBOX OFF

    stackoverflow r
    https://tinyurl.com/35wmvnut
    https://stackoverflow.com/questions/79230318/terradistance-between-point-and-polygon-returns-degrees-instead-of-km

    github
    https://tinyurl.com/2bdk4syj
    https://github.com/rogerjdeangelis/utl-computing-the-minimum-distance-between-a-polygon-and-a-point-gis-graph-plot-ai

    Related Reros

    https://github.com/rogerjdeangelis/utl-AI-internal-angles-of-polygon-from-vertex-coordinates-in-r
    https://github.com/rogerjdeangelis/utl-AI-labeling-centroids-inside-and-within-a-boundary-polygon
    https://github.com/rogerjdeangelis/utl-area-of-intersection-of-arbitrary-polygons-R-AI
    https://github.com/rogerjdeangelis/utl-calculate-the-area-within-a-latittude-longitude-polygon
    https://github.com/rogerjdeangelis/utl-draw-polygons-around-clusters-of-points-r-convex-hulls
    https://github.com/rogerjdeangelis/utl-how-many-triangles-in-the-polygon-r-igraph-AI
    https://github.com/rogerjdeangelis/utl-locate-the-centroid-point-of-a-polygon-r
    https://github.com/rogerjdeangelis/utl_AI_minimum_distance_from_a_poin_to_a_polygon
    https://github.com/rogerjdeangelis/utl_convex_hull_polygons_encompassing_a_three_dimensional_scatter_plot
    https://github.com/rogerjdeangelis/utl_simple_convex_hull_polygon_envelop_for_a_scatter_plot
    https://github.com/rogerjdeangelis/utl-AI-compute-the-distance-between-objects-in-an-image-python
    https://github.com/rogerjdeangelis/utl-AI-computer-vision-fitting-a-circle-to-a-scatter-plot-of-points-wps-r
    https://github.com/rogerjdeangelis/utl-AI-geometry-is-the-figure-a-right-triangle-
    https://github.com/rogerjdeangelis/utl-AI-internal-angles-of-polygon-from-vertex-coordinates-in-r
    https://github.com/rogerjdeangelis/utl-AI-labeling-centroids-inside-and-within-a-boundary-polygon
    https://github.com/rogerjdeangelis/utl-AI-remove-noise-from-an-image-python-opencv
    https://github.com/rogerjdeangelis/utl-capturing-old-faithful-before-and-during-an-eruption--AI-visual-analytics
    https://github.com/rogerjdeangelis/utl-python-AI-color-frequencies-in-an-image
    https://github.com/rogerjdeangelis/utl-R-AI-igraph-list-connections-in-a-non-directed-graph-for-a-subset-of-vertices
    https://github.com/rogerjdeangelis/utl-r-compute-the-area--of-an-image-which-is-under-a-curve-AI-image-processing-AI
    https://github.com/rogerjdeangelis/utl-r-python-compute-the-area-between-two-curves-AI-sympy-trapezoid


    /*               _     _
     _ __  _ __ ___ | |__ | | ___ _ __ ___
    | `_ \| `__/ _ \| `_ \| |/ _ \ `_ ` _ \
    | |_) | | | (_) | |_) | |  __/ | | | | |
    | .__/|_|  \___/|_.__/|_|\___|_| |_| |_|
    |_|
    */

    /**************************************************************************************************************************/
    /*                                                   |                                        |                           */
    /*            INPUT (TWO MACRO VARIABLES)            |            PROCESS                     | OUTPUT                    */
    /*                                                   |                                        |                           */
    /*                                                   |                                        |                           */
    /* %let poly=%str(1 1, 3 1, 3 2, 4 3, 3 4, 2 4, 1 1);| %utl_pybeginx;                         |DISTANCE=1.118033988749895 */
    /* %let pnt=3.5 5;                                   | parmcards4;                            |                           */
    /*                                                   | import pyperclip                       |SAS MCRO VARIABLE DISTANCE */
    /*                                                   | from shapely import wkt;               |                           */
    /*                                                   | poly = wkt.loads("POLYGON ((&poly))"); |%put &=distance;           */
    /*                         X                         | pt = wkt.loads("POINT(&pnt)");         |                           */
    /*      1.0   1.5   2.0   2.5   3.0   3.5   4.0      | dist=poly.distance(pt);                |DISTANCE=1.118033988749895 */
    /*   Y --+-----+-----+-----+-----+-----+-----+--- Y  | print (dist);                          |                           */
    /*     |                                        |    | pyperclip.copy(dist)                   |ie                         */
    /*     |                          .5   (5,3.5)  |    | ;;;;                                   |                           */
    /*   5 + sqrt(1^2 + .5^2) =1.118 -----+         + 5  | %utl_pyendx(resolve=Y,return=distance);|Pythagorean theorem check  */
    /*     |                         |   /          |    |                                        |sqrt(1*2 + .5**2) =1.118   */
    /*     |                       1 |  /           |    | %put &=distance;                       |                           */
    /*     |                         | / Find this  |    |                                        |                           */
    /*     |                         |/ Distance    |    |                                        |                           */
    /*   4 +                +--------+              + 4  |                                        |                           */
    /*     |               /    (3,4) \             |    |                                        |                           */
    /*     |              /            \            |    |                                        |                           */
    /*     |             /              \           |    |                                        |                           */
    /*     |            /                \          |    |                                        |                           */
    /*   3 +           /                  +         + 3  |                                        |                           */
    /*     |          /                  /          |    |                                        |                           */
    /*     |         /                  /           |    |                                        |                           */
    /*     |        /                  /            |    |                                        |                           */
    /*     |       /                  /             |    |                                        |                           */
    /*   2 +      /                  +              + 2  |                                        |                           */
    /*     |     /                   |              |    |                                        |                           */
    /*     |    /                    |              |    |                                        |                           */
    /*     |   /                     |              |    |                                        |                           */
    /*     |  /                      |              |    |                                        |                           */
    /*   1 + +-----------------------+              + 1  |                                        |                           */
    /*     |                                        |    |                                        |                           */
    /*     --+-----+-----+-----+-----+-----+-----+---    |                                        |                           */
    /*      1.0   1.5   2.0   2.5   3.0   3.5   4.0      |                                        |                           */
    /*                         X                         |                                        |                           */
    /*                                                   |                                        |                           */
    /**************************************************************************************************************************/

    /*                   _
    (_)_ __  _ __  _   _| |_
    | | `_ \| `_ \| | | | __|
    | | | | | |_) | |_| | |_
    |_|_| |_| .__/ \__,_|\__|
            |_|
    */

    %let poly=%str(1 1, 3 1, 3 2, 4 3, 3 4, 2 4, 1 1);
    %let pnt=3.5 5;

    /**************************************************************************************************************************/
    /*                                                                                                                        */
    /* %put &=poly;                                                                                                           */
    /*                                                                                                                        */
    /*   POLY=1 1, 3 1, 3 2, 4 3, 3 4, 2 4, 1 1                                                                               */
    /*                                                                                                                        */
    /*                                                                                                                        */
    /* %put &=pnt;                                                                                                            */
    /*                                                                                                                        */
    /*   PNT=3.5 5                                                                                                            */
    /*                                                                                                                        */
    /**************************************************************************************************************************/


    /*
     _ __  _ __ ___   ___ ___  ___ ___
    | `_ \| `__/ _ \ / __/ _ \/ __/ __|
    | |_) | | | (_) | (_|  __/\__ \__ \
    | .__/|_|  \___/ \___\___||___/___/
    |_|
    */

    %utl_pybeginx;
    parmcards4;
    import pyperclip
    from shapely import wkt;
    poly = wkt.loads("POLYGON ((&poly))");
    pt = wkt.loads("POINT(&pnt)");
    dist=poly.distance(pt);
    print (dist);
    pyperclip.copy(dist)
    ;;;;
    %utl_pyendx(resolve=Y,return=distance);

    %put &=distance;


    /**************************************************************************************************************************/
    /*                                                                                                                        */
    /* %put &=distance;                                                                                                       */
    /*                                                                                                                        */
    /* DISTANCE=1.118033988749895                                                                                             */
    /*                                                                                                                        */
    /**************************************************************************************************************************/

    /*              _
      ___ _ __   __| |
     / _ \ `_ \ / _` |
    |  __/ | | | (_| |
     \___|_| |_|\__,_|

    */

