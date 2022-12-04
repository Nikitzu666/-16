Выполнил: Смирнов Н.М.

Группа: ЭВТ-70

Игровой движок: Unity 2021.3.15

Название работы: разработка игры UI интерфейса

Лабораторная работа №16

Тема: Разработка анимированного UI интерфейса

Цель: Разработка анимированного UI интерфейса

Оборудование: компьютер.

Ход работы

1. Выполнение работы

Ищем на любом доступном сайте подходящие нам иконки для кнопок и всего остального в UI интерфейсе
![image](https://user-images.githubusercontent.com/119733911/205500368-f2e1c6b6-d0a4-45e6-8961-647595d355f1.png)
Рисунок 16.1 Нашли кнопки

Настраиваем Canvas и меняем режим рендеринга, так же настраиваем разрешение в котором будет работать наша игра
![image](https://user-images.githubusercontent.com/119733911/205500372-37fb6596-57ad-4130-88dd-9f8f63871dee.png)
Рисунок 16.2 Настроили Canvas

Настраиваем Background, привязываем бг к размеру экрана. И пишем с помощью Canvas название своей игры на нашем фоне.
![image](https://user-images.githubusercontent.com/119733911/205500378-6ac60dcd-1f73-41b3-a516-c9aad13b5260.png)
Рисунок 16.3 Настроили Background 

Добавляем спрайты кнопок которые будут использоваться в нашем меню.
![image](https://user-images.githubusercontent.com/119733911/205500382-cdc81f87-bdda-4c45-9e60-77f3166db856.png)
Рисунок 16.4 Спрайты кнопок

Делаем возможным создание анимаций на кнопки с помощью настроек кнопки
![image](https://user-images.githubusercontent.com/119733911/205500397-8de64d69-8982-4185-bbbb-b80cfcf8a3a0.png)
Рисунок 16.5 Создание анимаций

Настроили анимацию увеличения при наведении на кнопку Play
![image](https://user-images.githubusercontent.com/119733911/205500406-675fcfef-0625-4e9a-9806-f2b0fc6e450a.png)
Рисунок 16.6 Анимация увеличения

Настроили анимацию выдвижного меню при наведении на кнопку 
![image](https://user-images.githubusercontent.com/119733911/205500412-8102abc7-93bb-4ceb-a3f8-77352a5df5cf.png)
Рисунок 16.7 Анимация выдвижения меню

Листинг 16.1 MenuManager.cs
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class MenuManager : MonoBehaviour {
    public GameObject Panel;
// Use This for initialization
Void Start () {
}
// Update is called once per frame
Void Update () {
}
Public void Settings()
{
Panel.GetComponent<Animator>().SetTrigger(“Pop”);
}
}

2.Вывод
В ходе проделанной работы, мы разработали анимированный UI интерфейс.
