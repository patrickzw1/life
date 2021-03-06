# Life

***Summary***

The universe of the Game of Life is an infinite two-dimensional orthogonal grid of square cells. Each of square cells is in one of two possible states, alive or dead. Every cell interacts with eight neighbours. These neighbours are horizontally, vertically, or diagonally adjacent cells. At each step in time, the following transitions occur:

1. Any live cell with fewer than two live neighbours dies, as if caused by under-population.
2. Any live cell with two or three live neighbours lives on to the next generation.
3. Any live cell with more than three live neighbours dies, as if by overcrowding.
4. Any dead cell with exactly three live neighbours becomes a live cell, as if by reproduction.

The initial pattern constitutes the seed of the system. The first generation is created by applying the above rules simultaneously to every cell in the seed - births and deaths occur simultaneously, and the discrete moment at which this happens is sometimes called a tick (in other words, each generation is a pure function of the preceding one). The rules continue to be applied repeatedly to create further generations.

**Example**

```C
int glider[][2] = { {1,0}, {2,1}, {0,2}, {1,2}, {2,2} };
for( int i=0; i<5; i++ )
  4.     set_pixel( img, w, h, glider[i][0], glider[i][1], 255 );
5.
6. for( int i=0; i<32; i++ ) 7. {
  8.       draw_image_grey( img, w, h );
  9.       life( img, w, h );
 10.     }
 11.   draw_image_grey( img, w, h ); 
```

## Picture
![](https://github.com/OkeyDokeyYooo/life/blob/master/1.png)
![](https://github.com/OkeyDokeyYooo/life/blob/master/2.png)
