Заполнение файла style.stylus:
Задаются переменные header-color, sider-color и border-color. Если theme меняется на dark, то меняется на темную тему



h_header = 10vh
theme = 'light'

    header-color = #ff99ff
    border-color = #f070f0
    sider-color = #99ffff

if (theme == 'dark')
    header-color = #881188
    border-color = #200020
    sider-color = #559999

.main
    display flex
    flex-direction row
    height (100vh - h_header)
    width: 100%

.sider

    width: 15%
    border: 2px solid border-color
    background-color: sider-color

.header

    border: 2px solid border-color
    width 100%
    height h_header
    background-color: header-color
    margin-bottom: 5px

.content

    flex-grow: 1
    border: 2px solid border-color
    margin: 0px 10px
