
**背景介绍**


人工生命（AL:Artificial life）这一概念由美国计算机科学家、人工生命领域创始人之一克里斯托弗・盖尔・兰顿（Christopher G. Langton）提出。1986 年，兰顿提出了 “兰顿蚂蚁”（Langton's ant），它作为一个细胞自动机例子，是具有简单逻辑规则却能展现复杂动态行为的二维图灵机。次年，即 1987 年，在洛斯阿拉莫斯国家实验室（Los Alamos National Laboratory，制造了第一枚原子弹实验室）召开的 “生成以及模拟生命系统的国际会议” 上，兰顿正式提出了 “人工生命” 的概念，即使用计算机技术对生命建模，模拟生命系统。


目前人工生命的概念涵盖两个主要方面：其一为计算机科学范畴内的虚拟生命系统，这需要运用计算机软件工程以及人工智能技术来构建与实现；其二是借助基因工程技术对生物进行人工改造所形成的工程生物系统，其发展与合成生物学技术紧密相连，通过对生物遗传物质的精准操作与设计，赋予生物新的特性和功能，从而拓展生命的边界与可能性，推动生命科学在工程应用领域的进一步发展。


 


### 一、兰顿蚂蚁基本概念


* 定义：兰顿蚂蚁是一个二维图灵机，由黑白格子和一只“蚂蚁”构成。
* 提出者：克里斯托夫·兰顿
* 特性：拥有非常简单的逻辑和复杂的表现，其图灵完备性在2000年被证明。


### 二、规则与行为模式


* 规则：


	1. 在平面上的正方形格子中，每个格子被填上黑色或白色。
	2. 有一只“蚂蚁”位于其中一个格子上，其头部朝向上下左右其中一方。
	3. 若蚂蚁在白格上，则左转90度，将该格改为黑格，然后向前移一步。
	4. 若蚂蚁在黑格上，则右转90度，将该格改为白格，然后向前移一步。
* 行为模式：


	1. 初始阶段：从全白的背景开始，蚂蚁在最初的数百步内会留下许多对称或重复的形状的路线。例如，假设蚂蚁初始位于一个全白平面的中心格点，头部朝上，第一步它左转90度（因为在白格上），将所在格染黑，然后向前一步。这样几步下来就可能形成一个简单的对称图案。
	2. 混沌阶段：随着步数的增加，蚂蚁的路线会变得类似混沌的假随机状态。这一阶段蚂蚁的行走路线看起来毫无规律，就像随意乱走一样。
	3. 高速公路阶段：大约经过一万步后，蚂蚁的路线会进入一个以104步为周期的无限重复的“高速公路”模式，并朝固定方向移动。如下图所示：
	![](https://img2024.cnblogs.com/blog/785716/202412/785716-20241226112859336-1185318889.png)


### 三、推广与扩展


* 多种颜色：除了基本的黑白两色外，兰顿蚂蚁的概念也可以被扩展到使用多种颜色。每种颜色可以定义蚂蚁左转或右转的规则，通用的表示方法是用L和R依序表示各颜色是左转还是右转。
* 其他形状：除了正方形格子外，也可以使用其他形状的格子，如六角形格子。
* Turmites：进一步扩展是考虑Turing机器的多种状态，即蚂蚁本身的颜色可以改变。这些蚂蚁被称为“Turmites”，它们的行为模式包括产生高速公路、混乱增长和螺旋增长等。


### 四、意义与应用


* 理论意义：兰顿蚂蚁展示了简单规则下产生的复杂行为，对于理解细胞自动机、复杂系统和图灵机等领域具有重要意义。
* 实际应用：
	1. 计算布尔电路：兰顿蚂蚁的轨迹可以用于计算布尔电路，通过特定的初始配置，可以实现逻辑门的功能。比如在特定的黑白格初始布局下，蚂蚁的行走轨迹能对应布尔电路中的与、或、非等逻辑操作。
	2. 模拟图灵机：兰顿蚂蚁可以模拟任意图灵机进行计算，显示了其通用计算能力。例如，通过设计特定的初始状态，如设定某些格子的颜色以及蚂蚁的初始位置和朝向等，可以实现简单的图灵机算法。
	3. 模式生成：在艺术和设计领域，兰顿蚂蚁的轨迹可以生成独特的图案和纹理，用于装饰和创意设计。例如，将蚂蚁的行走轨迹记录下来，经过艺术化处理后可以成为独特的壁纸图案。


### 五、与其他模型的对比


* 与Conway的生命游戏对比：Conway的生命游戏也是一个经典的细胞自动机模型，但它主要关注的是细胞的生存和繁殖规则，而兰顿蚂蚁则更注重个体行为的动态变化和路径生成。
* 与元胞自动机对比：元胞自动机通常涉及多个细胞的状态变化，而兰顿蚂蚁则专注于单个“蚂蚁”的行为，尽管规则简单，但产生的行为却异常复杂。
* 与图灵机对比：图灵机是一种通用计算模型，而兰顿蚂蚁通过简单的规则实现了图灵完备性，展示了简单系统中的复杂计算能力。


**下面是代码：**


兰顿蚂蚁html\\go\\php\\python\\java


每个版本都实现了相同的功能：


在网格上模拟兰顿蚂蚁的移动


使用黑白两色表示网格状态


用红色标记蚂蚁当前位置


支持周期性边界条件


![](https://img2024.cnblogs.com/blog/785716/202412/785716-20241226111110596-1682225258.png)


 


HTML版本：




```
DOCTYPE html>
<html>
<head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    <title>兰顿蚂蚁title>
    <style>
        html, body {
            margin: 0 !important;
            padding: 0 !important;
        }
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: #555555;
            height: 100vh;
        }
        canvas {
            display: block;
            background-color: white;
        }
        #temp {
            display: none;
        }
    style>
head>
<body>
    <canvas id="bg" width="640" height="640">canvas>
    <canvas id="temp" width="640" height="640">canvas>
    <script>
        // 处理索引边界
        const cycle = (idx, max) => (idx + max) % max;

        // 获取画布和上下文
        const bg = document.getElementById("bg");
        const temp = document.getElementById("temp");
        const ctx = bg.getContext("2d");
        const ctempx = temp.getContext("2d");

        // 设置基本参数
        const bgWidth = 640;
        const bgHeight = 640;
        const size = 2;
        const speed = 100;
        const width = bgWidth / size;
        const height = bgHeight / size;

        // 初始化画布尺寸
        [bg, temp].forEach(canvas => {
            canvas.width = bgWidth;
            canvas.height = bgHeight;
        });

        // 蚂蚁初始位置（中心点）
        let antx = width / 2;
        let anty = height / 2;

        // 方向数组：上、右、下、左
        const dirs = [[0, -1], [1, 0], [0, 1], [-1, 0]];
        let dir = 0;

        // 初始化网格（使用数组技巧）
        let grid = new Array(height).fill(0).map(_ => new Array(width).fill(1));

        // 移动函数（dir可以是负数或大于3）
        const move = (dir) => {
            dir = cycle(dir, dirs.length);
            antx += dirs[dir][0];
            anty += dirs[dir][1];
            antx = cycle(antx, width);
            anty = cycle(anty, height);
            return dir;
        }

        // 初始化画布设置
        ctx.fillStyle = "white";
        ctx.fillRect(0, 0, bgWidth, bgHeight);
        ctx.scale(size, size);
        ctx.imageSmoothingEnabled = false;

        // 单步执行函数
        const step = () => {
            const px = grid[anty][antx];
            // 翻转当前格子的颜色，然后移动到下一个格子
            if (px > 0) {
                grid[anty][antx] = 0;  // 变黑
                dir = move(dir + 1);    // 右转
            } else {
                grid[anty][antx] = 7;  // 变白
                dir = move(dir - 1);    // 左转
            }
        }

        // 颜色转换函数
        const intToColor = (px) => {
            // 颜色对应关系：
            // 0 -> 黑色 [0, 0, 0] * 255
            // 7 -> 白色 [1, 1, 1] * 255
            // 3 -> 红色 [1, 0, 0] * 255
            // 最后一个字节是透明度
            return [px % 2 * 255, px % 3 * 255, px % 3 * 255, 255];
        }

        // 绘制函数
        const paint = () => {
            // 在渲染前计算多步
            for (let i = 0; i < speed; i++) {
                step();
            }
            // 用红色标记蚂蚁的位置
            const tmp = grid[anty][antx];
            grid[anty][antx] = 3;
            const bytes = grid.flat().map(intToColor).flat();
            const imgData = new ImageData(Uint8ClampedArray.from(bytes), width, height);
            grid[anty][antx] = tmp;
            ctempx.putImageData(imgData, 0, 0);
            ctx.drawImage(temp, 0, 0);
        }

        // 设置动画循环
        setInterval(paint, 20);
    script>
body>
html>
```


Python版本使用Pygame库实现图形界面，要运行这些代码你需要安装相应的依赖： Python: pip install pygame




```
import pygame
import numpy as np

# 初始化 Pygame
pygame.init()

# 设置基本参数
BG_WIDTH = 640
BG_HEIGHT = 640
CELL_SIZE = 2
SPEED = 100
WIDTH = BG_WIDTH // CELL_SIZE
HEIGHT = BG_HEIGHT // CELL_SIZE

# 创建窗口
screen = pygame.display.set_mode((BG_WIDTH, BG_HEIGHT))
pygame.display.set_caption("兰顿蚂蚁")

# 初始化网格
grid = np.ones((HEIGHT, WIDTH), dtype=int)

# 蚂蚁初始位置（中心点）
ant_x = WIDTH // 2
ant_y = HEIGHT // 2

# 方向数组：上、右、下、左
DIRS = [(0, -1), (1, 0), (0, 1), (-1, 0)]
dir_idx = 0

def move(direction):
    global ant_x, ant_y
    direction = direction % len(DIRS)
    ant_x = (ant_x + DIRS[direction][0]) % WIDTH
    ant_y = (ant_y + DIRS[direction][1]) % HEIGHT
    return direction

def step():
    global dir_idx
    px = grid[ant_y][ant_x]
    if px > 0:
        grid[ant_y][ant_x] = 0  # 变黑
        dir_idx = move(dir_idx + 1)  # 右转
    else:
        grid[ant_y][ant_x] = 7  # 变白
        dir_idx = move(dir_idx - 1)  # 左转

def int_to_color(px):
    if px == 0:  # 黑色
        return (0, 0, 0)
    elif px == 7:  # 白色
        return (255, 255, 255)
    else:  # 红色（蚂蚁位置）
        return (255, 0, 0)

# 主循环
running = True
clock = pygame.time.Clock()

while running:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            running = False

    # 计算多步
    for _ in range(SPEED):
        step()

    # 绘制
    for y in range(HEIGHT):
        for x in range(WIDTH):
            color = int_to_color(grid[y][x])
            pygame.draw.rect(screen, color, 
                           (x * CELL_SIZE, y * CELL_SIZE, 
                            CELL_SIZE, CELL_SIZE))
    
    # 标记蚂蚁位置
    pygame.draw.rect(screen, (255, 0, 0),
                    (ant_x * CELL_SIZE, ant_y * CELL_SIZE,
                     CELL_SIZE, CELL_SIZE))

    pygame.display.flip()
    clock.tick(50)

pygame.quit()
```


 


Java版本使用Swing实现图形界面




```
import javax.swing.*;
import java.awt.*;
import java.awt.image.BufferedImage;

public class LangtonAnt extends JPanel {
    private static final int BG_WIDTH = 640;
    private static final int BG_HEIGHT = 640;
    private static final int CELL_SIZE = 2;
    private static final int SPEED = 100;
    private static final int WIDTH = BG_WIDTH / CELL_SIZE;
    private static final int HEIGHT = BG_HEIGHT / CELL_SIZE;

    private int[][] grid;
    private int antX, antY, dir;
    private final int[][] dirs = {{0, -1}, {1, 0}, {0, 1}, {-1, 0}};
    private BufferedImage buffer;

    public LangtonAnt() {
        setPreferredSize(new Dimension(BG_WIDTH, BG_HEIGHT));
        initializeGrid();
        buffer = new BufferedImage(WIDTH, HEIGHT, BufferedImage.TYPE_INT_RGB);
        
        Timer timer = new Timer(20, e -> {
            update();
            repaint();
        });
        timer.start();
    }

    private void initializeGrid() {
        grid = new int[HEIGHT][WIDTH];
        for (int y = 0; y < HEIGHT; y++) {
            for (int x = 0; x < WIDTH; x++) {
                grid[y][x] = 1;
            }
        }
        antX = WIDTH / 2;
        antY = HEIGHT / 2;
        dir = 0;
    }

    private int move(int direction) {
        direction = (direction + dirs.length) % dirs.length;
        antX = (antX + dirs[direction][0] + WIDTH) % WIDTH;
        antY = (antY + dirs[direction][1] + HEIGHT) % HEIGHT;
        return direction;
    }

    private void step() {
        int px = grid[antY][antX];
        if (px > 0) {
            grid[antY][antX] = 0;  // 变黑
            dir = move(dir + 1);   // 右转
        } else {
            grid[antY][antX] = 7;  // 变白
            dir = move(dir - 1);   // 左转
        }
    }

    private void update() {
        for (int i = 0; i < SPEED; i++) {
            step();
        }
    }

    @Override
    protected void paintComponent(Graphics g) {
        super.paintComponent(g);
        
        // 更新缓冲图像
        for (int y = 0; y < HEIGHT; y++) {
            for (int x = 0; x < WIDTH; x++) {
                buffer.setRGB(x, y, grid[y][x] > 0 ? 0xFFFFFF : 0);
            }
        }
        buffer.setRGB(antX, antY, 0xFF0000);  // 蚂蚁位置标记为红色

        // 绘制放大后的图像
        g.drawImage(buffer, 0, 0, BG_WIDTH, BG_HEIGHT, null);
    }

    public static void main(String[] args) {
        SwingUtilities.invokeLater(() -> {
            JFrame frame = new JFrame("兰顿蚂蚁");
            frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
            frame.add(new LangtonAnt());
            frame.pack();
            frame.setLocationRelativeTo(null);
            frame.setVisible(true);
        });
    }
}
```


 


Go版本使用Ebiten游戏引擎实现图形界面，要运行这些代码你需要安装相应的依赖： Go: go get github.com/hajimehoshi/ebiten/v2




```
package main

import (
    "image/color"
    "log"

    "github.com/hajimehoshi/ebiten/v2"
)

const (
    bgWidth  = 640
    bgHeight = 640
    cellSize = 2
    speed    = 100
    width    = bgWidth / cellSize
    height   = bgHeight / cellSize
)

type Game struct {
    grid    [][]int
    antX    int
    antY    int
    dir     int
    dirs    [][2]int
    pixels  []byte
}

func NewGame() *Game {
    g := &Game{
        grid: make([][]int, height),
        antX: width / 2,
        antY: height / 2,
        dirs: [][2]int{{0, -1}, {1, 0}, {0, 1}, {-1, 0}},
        pixels: make([]byte, width*height*4),
    }

    for y := range g.grid {
        g.grid[y] = make([]int, width)
        for x := range g.grid[y] {
            g.grid[y][x] = 1
        }
    }

    return g
}

func (g *Game) move(dir int) int {
    dir = (dir + len(g.dirs)) % len(g.dirs)
    g.antX = (g.antX + g.dirs[dir][0] + width) % width
    g.antY = (g.antY + g.dirs[dir][1] + height) % height
    return dir
}

func (g *Game) step() {
    px := g.grid[g.antY][g.antX]
    if px > 0 {
        g.grid[g.antY][g.antX] = 0 // 变黑
        g.dir = g.move(g.dir + 1)  // 右转
    } else {
        g.grid[g.antY][g.antX] = 7 // 变白
        g.dir = g.move(g.dir - 1)  // 左转
    }
}

func (g *Game) Update() error {
    for i := 0; i < speed; i++ {
        g.step()
    }
    return nil
}

func (g *Game) Draw(screen *ebiten.Image) {
    // 更新像素数据
    for y := 0; y < height; y++ {
        for x := 0; x < width; x++ {
            idx := (y*width + x) * 4
            if g.grid[y][x] > 0 {
                g.pixels[idx] = 255   // R
                g.pixels[idx+1] = 255 // G
                g.pixels[idx+2] = 255 // B
                g.pixels[idx+3] = 255 // A
            } else {
                g.pixels[idx] = 0     // R
                g.pixels[idx+1] = 0   // G
                g.pixels[idx+2] = 0   // B
                g.pixels[idx+3] = 255 // A
            }
        }
    }

    // 标记蚂蚁位置
    idx := (g.antY*width + g.antX) * 4
    g.pixels[idx] = 255   // R
    g.pixels[idx+1] = 0   // G
    g.pixels[idx+2] = 0   // B
    g.pixels[idx+3] = 255 // A

    screen.WritePixels(g.pixels)
}

func (g *Game) Layout(outsideWidth, outsideHeight int) (int, int) {
    return width, height
}

func main() {
    ebiten.SetWindowSize(bgWidth, bgHeight)
    ebiten.SetWindowTitle("兰顿蚂蚁")

    if err := ebiten.RunGame(NewGame()); err != nil {
        log.Fatal(err)
    }
}
```


 


PHP版本使用GD库生成静态图像，要运行这些代码你需要安装相应的依赖： PHP: 需要安装GD扩展




```
<span style="color: rgba(0, 0, 0, 1)"php

class LangtonAnt {
    private $width = 640;
    private $height = 640;
    private $cellSize = 2;
    private $speed = 100;
    private $gridWidth;
    private $gridHeight;
    private $grid = [];
    private $antX;
    private $antY;
    private $dir = 0;
    private $dirs = [[0, -1], [1, 0], [0, 1], [-1, 0]];
    private $image;

    public function __construct() {
        $this->gridWidth = $this->width / $this->cellSize;
        $this->gridHeight = $this->height / $this->cellSize;
        $this->antX = $this->gridWidth / 2;
        $this->antY = $this->gridHeight / 2;

        // 初始化网格
        for ($y = 0; $y < $this->gridHeight; $y++) {
            $this->grid[$y] = array_fill(0, $this->gridWidth, 1);
        }

        // 创建图像
        $this->image = imagecreatetruecolor($this->width, $this->height);
        imagefilledrectangle($this->image, 0, 0, $this->width, $this->height, 
                            imagecolorallocate($this->image, 255, 255, 255));
    }

    private function move($dir) {
        $dir = ($dir + count($this->dirs)) % count($this->dirs);
        $this->antX = ($this->antX + $this->dirs[$dir][0] + $this->gridWidth) % $this->gridWidth;
        $this->antY = ($this->antY + $this->dirs[$dir][1] + $this->gridHeight) % $this->gridHeight;
        return $dir;
    }

    private function step() {
        $px = $this->grid[$this->antY][$this->antX];
        if ($px > 0) {
            $this->grid[$this->antY][$this->antX] = 0;  // 变黑
            $this->dir = $this->move($this->dir + 1);   // 右转
        } else {
            $this->grid[$this->antY][$this->antX] = 7;  // 变白
            $this->dir = $this->move($this->dir - 1);   // 左转
        }
    }

    public function run($steps) {
        for ($i = 0; $i < $steps; $i++) {
            $this->step();
        }

        // 绘制网格
        for ($y = 0; $y < $this->gridHeight; $y++) {
            for ($x = 0; $x < $this->gridWidth; $x++) {
                $color = $this->grid[$y][$x] > 0 ? 
                    imagecolorallocate($this->image, 255, 255, 255) : 
                    imagecolorallocate($this->image, 0, 0, 0);
                
                imagefilledrectangle(
                    $this->image,
                    $x * $this->cellSize,
                    $y * $this->cellSize,
                    ($x + 1) * $this->cellSize - 1,
                    ($y + 1) * $this->cellSize - 1,
                    $color
                );
            }
        }

        // 标记蚂蚁位置
        $red = imagecolorallocate($this->image, 255, 0, 0);
        imagefilledrectangle(
            $this->image,
            $this->antX * $this->cellSize,
            $this->antY * $this->cellSize,
            ($this->antX + 1) * $this->cellSize - 1,
            ($this->antY + 1) * $this->cellSize - 1,
            $red
        );

        // 输出图像
        header('Content-Type: image/png');
        imagepng($this->image);
        imagedestroy($this->image);
    }
}

$ant = new LangtonAnt();
$ant->run(10000);  // 运行10000步
```


综上所述，兰顿蚂蚁是一个具有深刻理论意义和广泛应用前景的细胞自动机模型。它通过简单的规则展示了复杂的行为模式，为我们理解自然界和人工系统中的复杂现象提供了新的视角和工具。未来的研究可以进一步探索兰顿蚂蚁在更多领域的应用，如生物系统的建模、城市交通规划等，以及开发新的扩展模型，以增强其计算能力和表现形式。


 本博客参考[西部世界westwingy加速器](https://www.yicheer.com)。转载请注明出处！
