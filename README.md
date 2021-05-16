# Моя реализация Raycating
движек с видом от первого лица
(как в [Wolfenstein 3D](https://fr.wikipedia.org/wiki/Wolfenstein_3D)).

<img align="center" src="./screenshot.bmp" alt="Screenshot of the game" />

### Быстрый старт

``make && make clean && ./cub3D maps/dust.cub``

# Как запустить
В командной строке использовать команду ``make`` для создания ``cub3D`` исполняемого файла.

Запустить командой ``./cub3D maps/<имя карты> ``

доступные карты: dust.cub, winter.cub, forest.cub

## формат карты
``R 1240 720``                    разрешение

``NO textures/yellow_brick.xpm``  адрес северной текстуры

``SO textures/grey_brick.xpm``    адрес южной текстуры

``WE textures/wood.xpm``          адрес зарадной текстуры

``EA textures/red_brick.xpm``     адрес восточной текстуры

``S textures/sprites/barrel.xpm`` адрес текстуры спрайта

``F 230, 198, 110``               цвет пола в формате RGB

``C 152, 224, 235``               цвет потолка в формате RGB

Дальше идет сама карта, где ``1``- стена, ``0``- пустое пространство, ``E,N,W или S`` - позиция игрока(в зависимости от стороны света куда он смотрит), ``S`` - спрайт

### Управление

Перемещение вперед/влево/назад/вправо ``W`` ``A`` ``S`` ``D``.
Повороты вокруг в стороны ``←````→`` и ``Q`` ``E``.
"Бег" ``SHIFT``.
Чтобы выйти из игры ``ESC`` или нажать красный крестик.

## Статьи и сточники

* [Tutorial](https://lodev.org/cgtutor/raycasting.html)
* [Wolfenstein 3D](http://users.atw.hu/wolf3d/)
* [X11](https://github.com/qst0/ft_libgfx)
* [BMP format](https://web.archive.org/web/20080912171714/http://www.fortunecity.com/skyscraper/windows/364/bmpffrmt.html)
* [42 Docs](https://harm-smits.github.io/42docs/)
