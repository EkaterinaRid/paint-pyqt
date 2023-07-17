Суть работы: Создание программы, способной изображать некоторые графические примитивы.

Функции: Прямоугольник, закругленный прямоугольник, эллис, ручка, спрей, прямая, точка, сектор, дуга, многоугольник, круговой сегмент, текст, изображение, а также настройка ширины и цвета.

Описание реализации:
Будут реализованы 3 класса объектов:
PaletteButton, наследующийся от QPushButton – кнопка, с помощью которой определяется цвет кисти.
Canvas, наследующийся от Qlabel – холст, на котором все будет рисоваться. В нем будут реализованы методы рисования графических примитивов и обработки картинок.
MainWindow, наследующийся от QMainWindow – окно, в котором отображены холст, палитра цветов и функции, реализованные в программе. С помощью MainWindow осуществляется взаимодействие пользователя с методами Canvas и регулирование цвета кисти.
Будет реализована функция resize_image, которая работает с модулем ffmpeg (аналог PIL из Python) и масштабирует выбранную картинку под размеры холста и регулирует ее размеры при ее сохранении.
Будет использован модуль random, помогающий реализовать спрей.
