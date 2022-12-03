# LR-16[LR-16.zip](https://github.com/Maxsim2418/LR-16/files/10146045/LR-16.zip)

Борнеман М.А

ЭВТ-70

Игровой движок:Unity

Лабораторная работа №16

Тема: Разработка анимированного UI интерфейса

Цель: приобрести навыки в разработке UI интерфейса

Ход работы:

1.	Выполнение работы

1.	Был установлен background, была добавлен заголовок игры, были добавлены кнопки, а также анимации для кнопки «Play» и «Settings»

![image](https://user-images.githubusercontent.com/119674602/205433057-cc61a888-1541-4a48-99f6-eb2be4c6c928.png)

Рисунок 16.1 – Постройка сцены.

2.	Был добавлен скрипт для добавления тригера в панель настроек, и для того,что бы задать ссылку, которая будет открываться при нажатии на кнопку «Share».

Листинг 16.1 MenuManager.cs

using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class MenuManager : MonoBehaviour
{
    public GameObject panel;

    public void Settings()
    {
        panel.GetComponent<Animator>().SetTrigger("Pop");
    }

    public void OpenSite()
    {
        Application.OpenURL("http://wikipedia.org/");
    }
}

2.	Вывод

В ходе проделанной работы был разработан анимированный UI интерфейс. 
