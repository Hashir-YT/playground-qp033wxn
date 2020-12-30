//player moves 
int moveLeft = 0;
int enemyMove = 5; 
Random rnd = new Random(); 
int bulletSpeed = 8;
bool shooting = false; 
int score = 0;
public Form1()
 
{
 
InitializeComponent(); enemy1.Top = -500;
enemy2.Top = -900;
enemy3.Top = -1300;
 
bullet.Top = -100;
 
bullet.Left = -100;
 
}
if(e.KeyCode == Keys.Left)
 
{
 
if (player.Location.X< 0)
 
{
 
moveLeft = 0;
 
}
 
else
 
{
 
moveLeft = -5;
 
}
 
}
else if(e.KeyCode == Keys.Right)
 
{
 
if (player.Location.X> 512)
 
{
 
moveLeft = 0;
 
}
 
else
 
{
 
moveLeft = 5;
 
}
 
}
else if (e.KeyCode == Keys.Space)
{
 
if (shooting == false)
{
bulletSpeed = 8;
bullet.Left = player.Left + 50; bullet.Top = player.Top;
shooting = true;
 
}
}
if (e.KeyCode == Keys.Left)
 
{
 
moveLeft = 0;
 
}
 
else if (e.KeyCode == Keys.Right)
 
{
 
moveLeft = 0;
 
}