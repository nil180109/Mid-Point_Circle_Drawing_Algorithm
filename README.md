# Mid-Point_Circle_Drawing_Algorithm

The mid-point circle drawing algorithm is an algorithm used to determine the points needed for rasterizing a circle. 
 

We use the mid-point algorithm to calculate all the perimeter points of the circle in the first octant and then print them along with their mirror points in the other octants. This will work because a circle is symmetric about its centre.

 

Circle octants

 

The algorithm is very similar to the Mid-Point Line Generation Algorithm. Here, only the boundary condition is different.

 

For any given pixel (x, y), the next pixel to be plotted is either (x, y+1) or (x-1, y+1). This can be decided by following the steps below.

 

Find the mid-point p of the two possible pixels i.e (x-0.5, y+1)
If p lies inside or on the circle perimeter, we plot the pixel (x, y+1), otherwise if it’s outside we plot the pixel (x-1, y+1)
Boundary Condition : Whether the mid-point lies inside or outside the circle can be decided by using the formula:- 
 

Given a circle centered at (0,0) and radius r and a point p(x,y) 
F(p) = x2 + y2 – r2 
if F(p)<0, the point is inside the circle
F(p)=0, the point is on the perimeter
F(p)>0, the point is outside the circle 
