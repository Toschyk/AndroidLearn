# AndroidLearn
# Глава 1. Начало работы с Android
## 1.1 Java и Android | Введение. Установка Android Studio и Android SDK

Бурное развитие информационных технологий в последнее время привело к тому, что появилось много новых устройств и технологий, таких, как планшеты, смартфоны, нетбуки, другие гаджеты. Они все более прочно входят в нашу жизнь и становятся привычным делом. Лидирующей платформой среди подобных гаджетов на сегодняшний день является ОС Андроид.

Android используется на самых разных устройствах. Это и смартфоны, и планшеты, и телевизоры, и смарт-часы и ряд других гаджетов. По разным подсчетам за 2020 год этой операционой системой пользуются около 85% владельцев смартфонов, а общее количество пользователей сматрфонов на ОС Android оценивается в более чем 2,5 млрд. человек по всему миру.

ОС Андроид была создана разработчиком Энди Рубином (Andy Rubin) в качестве операционной системы для мобильных телефонов и поначалу развивалась в рамках компании Android Inc. Но в 2005 году Google покупает Android Inc. и начинает развивать операционную систему с новой силой. Android постоянно эволюционирует, и вместе с операционной системой эволюционируют средства и инструменты для разработки. На данный момент (ноябрь 2024 года) последней версией является Android 15.0, которая вышла в сентябре 2024 года:


| Версия  | Кодовое имя | Дата выпуска | Уровень API |
| ------------- | ------------- | ------------- | ------------- |
| 15.0  | Vanilla Ice Cream  |  3 сентября 2024 года  | 35  | 
| 14.0  | Upside Down Cake  | 4 сентября 2023  | 34  | 
| 13.0 | Tiramisu | 15 августа 2022 | 33  | 
| 12L | Snow Cone  | март 2022 | 32  | 
| 12.0 | Snow Cone | 4 октября 2021 | 31  | 
| 11.0 | Red Velvet Cake | 8 сентября 2020 | 30  | 
| 10.0 | Quince Tart  | 3 сентября 2019 | 29  | 
| 9.0 | Pie | 6 августа 2018 | 28  | 
| 8.1 | Oreo | 5 декабря 2017 | 27  | 
| 8.0 | Oreo | 21 августа 2017 | 26  | 
| 7.1 | Nougat | 4 октября 2016 | 25  | 
| 7.0 | Nougat | 22 августа 2016 | 24  | 
| 6.0 | Marshmallow | 5 октября 2015 | 23  | 
| 5.1 | Lollipop | 9 марта 2015 | 22  | 
| 5.0 | Lollipop | 3 ноября 2014 | 21  | 
| 4.4 | KitKat | 31 октября 2013 | 19  | 
| 4.3 | Jelly Bean | 24 июля 2013 | 18  | 
| 4.2 | Jelly Bean  | 13 ноября 2012 | 17  | 
| 4.1 | Jelly Bean | 9 июля 2012 | 16  | 
| 4.0 | Ice Cream Sandwich | 16 декабря 2011 | 15  | 
| 2.3 | Gingerbread | 6 декабря 2010  | 	10  | 

### Что нужно для разработки?

Стоит отметить, что разрабатывать приложения под Android можно с помощью различных фреймворков и языков программирования. Так, в качестве языков программирования могут применяться Java, Kotlin, Dart (фреймворк Flutter), C++, Python, C# (платформа Xamarin/MAUI), JavaScript (React Native) и т.д. В данном руководстве мы будем использовать именно язык Java, как наиболее распространенный и используемый. Поэтому прежде чем приступать к освоению программирования под Android по данному руководству, необходимо освоить хотя бы базовые момент языка Java.

### Установка средств разработки

Существуют разные среды разработки для Android. Рекомендуемой средой разработки является Android Studio, которая создана специально для разработки под ОС Android. Поэтому мы ее и будем использовать. Загрузить файл установщика можно с официального сайта: https://developer.android.com/studio

Кроме самой среды Android Studio для разработки также потребуется набор инструментов, который называется Android SDK. Например, если ранее Android SDK еще не было установлено, то при первом обращении к Android Studio она предложит установить ряд дополнительных инструментов, которые необходимы для разработки. Прежде всего это Android SDK и ряд дополнительных компонентов.

Нажмем на кнопку Finish, чтобы, наконец, все это установить.

И после завершения установки нажмем на кнопку Finish. И мы можем приступать к созданию приложений.

## 1.2 Java и Android | Первый проект в Android Studio

Теперь создадим первое приложение в среде Android Studio для операционной системы Android. Откроем Android Studio и на начальном экране выберем пункт New Project.

При создании проекта Android Studio вначале предложит нам выбрать шаблон проекта.

Android Studio предоставляет ряд шаблонов для различных ситуаций. Для создания приложения на Java выберем в этом списке шаблон Empty Views Activity, который предоставляет самый простейший фукционал, необходимый для начала, и нажмем на кнопку Next.

После этого отобразится окно настроек нового проекта.

В окне создания нового проекта мы можем установить его начальные настройки:

  -  В поле Name вводится название приложения. Укажем в качестве имени название HelloApp

  -  В поле Package Name указывается имя пакета, где будет размещаться главный класс приложения. В данном случае для тестовых проектов это значение не играет ольшого значения, поэтому установим com.example.helloapp.

  -  В поле Save Location установливается расположение файлов проекта на жестком диске. Можно оставить значение по умолчанию.

  -  В поле Language в качестве языка программирования укажем Java (будьт внимательны, так как по умолчанию в этом поле стоит Kotlin)

  -  В поле Minimum SDK указывается самая минимальная поддерживаемая версия SDK. Оставим значение по умолчанию. Минимальная версия означает, что наше приложение можно будет запустить начиная с этой версии. На более старых устройствах запустить будет нельзя.

     Стоит учитывать, что чем выше версия SDK, тем меньше диапазон поддерживаемых устройств.

Далее нажмем на кнопку Finish, и Android Studio создаст новый проект.

Вначале вкратце рассмотрим структуру проекта, что он уже имеет по умолчанию.

Проект Android может состоять из различных модулей. По умолчанию, когда мы создаем проект, создается один модуль - app. Модуль имеет три подпапки:

  -  manifests: хранит файл манифеста AndroidManifest.xml, который описывает конфигурацию приложения и определяет каждый из компонентов данного приложения.

  -  java: хранит файлы кода на языке java, которые структурированы по отдельным пакетам. Так, в папке com.example.helloapp (название которого было указано на этапе создания проекта) имеется по умолчанию файл MainActivity.java с кодом на языке Java, который представляет класс MainActivity, запускаемый по умолчанию при старте приложения

  -  res: содержит используемые в приложении ресурсы. Все ресурсы разбиты на подпапки.

     -   папка drawable предназначена для хранения изображений, используемых в приложении

     -   папка layout предназначена для хранения файлов, определяющих графический интерфейс. По умолчанию здесь есть файл activity_main.xml, который определяет интерфейс для класса MainActivity в виде xml

      -  папки mipmap содержат файлы изображений, которые предназначены для создания иконки приложения при различных разрешениях экрана.

      -  папка values хранит различные xml-файлы, содержащие коллекции ресурсов - различных данных, которые применяются в приложении. По умолчанию здесь есть два файла и одна папка:

         -   файл colors.xml хранит описание цветов, используемых в приложении

         -   файл strings.xml содержит строковые ресурсы, используемые в приложении

         -   папки themes хранит две темы приложения - для светлую (дневную) и темную (ночную)

Отдельный элемент Gradle Scripts содержит ряд скриптов, которые используются при построении приложения.

Во всей этой структуре следует выделить файл MainActivity.java, который открыт в Android Studio и который содержит логику приложения и собственно с него начинается выполнение приложения. И также выделим файл activity_main.xml, который определяет графический интерфейс - по сути то, что увидит пользователь на своем смартфоне после загрузки приложения.

### Запуск проекта

Созданный выше проект уже содержит некоторый примитивный функционал. Правда, этот функционал почти ничего не делает, только выводит на экран строку "Hello world!". Тем не менее это уже фактически приложение, которое мы можем запустить.

Для запуска и тестирования приложения мы можем использовать эмуляторы или реальные устройства. Но в идеале лучше тестировать на реальных устройствах. К тому же эмуляторы требуют больших аппаратных ресурсов, и не каждый компьютер может потянуть требования эмуляторов. А для использования мобильного устройства для тестирования может потребоваться разве что установить необходимый драйвер.

### Режим разработчика на телефоне

По умолчанию опции разработчика на смартфонах скрыты. Чтобы сделать их доступными, надо зайти в Settings > About phone (Настройки > О телефоне) (в Android 8 это в Settings > System > About phone (Настройки > Система > О телефоне)) и семь раз нажать Build Number (Номер сборки).

Теперь необходимо включить отладку по USB. Для этого перейдем в Settings > System > Advanced > Developer options или Настройки > Система > Дополнительно > Для разработчиков (в Android 8 это в Settings > System > Developer options или Настройки > Система > Для разработчиков ).

И включим возможность отладки по USB.

### Запуск приложения

Подключим устройство с ОС Android (если мы тестируем на реальном устройстве) и запустим проект, нажав на зеленую стрелочку на панели инструментов.

Выберем устройство и нажмем на кнопку OK. И после запуска мы увидим наше приложение на экране устройства.

## 1.3 Java и Android | Создание графического интерфейса

В прошлой теме мы рассмотрели создание простого приложения, который предлагает Android Studio по умолчанию и которое просто выводит на экран строку Hello Android.

Но почему у нас выводится именно эта строка? Почему у нас вообще создается именно такой визуальный интерфейс?

Выполнение приложения Android по умолчанию начинается с класса MainActivity, который по умолчанию открыт в Android Studio:

```java
package com.example.helloapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
}
```

Каждый отдельный экран или страница в приложении описывается таким понятием как activity. В литературе могут использоваться различные термины: экран, страница, активность. В данном случае я буду использовать понятие "activity". Так вот, если мы запустим приложение на устройстве, то на экране мы по сути увидим определенную activity, которая предсталяет данный интерфейс.

Класс MainActivity по сути представляет обычный класс java, в начале которого идет определение пакета данного класса:

```java
package com.example.helloapp;
```

Далее идет импорт классов из других пакетов, функциональность которых используется в MainActivity:

```java
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
```

Затем идет собственно определение класса:

```java
public class MainActivity extends AppCompatActivity
```

По умолчанию MainActivity наследуется от класса AppCompatActivity, который выше подключен с помощью директивы импорта. Класс AppCompatActivity по сути представляет отдельный экран (страницу) приложения или его визуальный интерфейс. И MainActivity наследует весь этот функционал.

По умолчанию MainActivity содержит только один метод onCreate(), в котором фактически и создается весь интерфейс приложения:

```java
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
}
```

В метод setContentView() передается ресурс разметки графического интерфейса:

```java
setContentView(R.layout.activity_main);
```

Именно здесь и решается, какой именно визуальный интерфейс будет иметь MainActivity. Но что в данном случае представляет ресурс R.layout.activity_main? Это файл activity_main.xml из папки res/layout (в принципе можно заметить, что название ресурса соответствует названию файла), который также по умолчанию открыт в Android Studio:

### Файл activity_main.xml

Android Studio позволяет работать с визуальным интерфейсом как в режиме кода, так и в графическом режиме. Так, по умолчанию файл открыт в графическом режиме, и мы наглядно можем увидеть, как у нас примерно будет выглядеть экран приложения. И даже набрасать с панели инструментов какие-нибудь элементы управления, например, кнопки или текстовые поля.

Но также мы можем работать с файлом в режиме кода, поскольку activity_main.xml - это обычный текстовый файл с разметкой xml. Для переключения к коду нажмем на кнопку Code над графическим представлением. (Дополнительно с помощью кнопки Split можно переключиться на комбинированное представление код + графический дизайнер)

Здесь мы увидим, что на уровне кода файл activity_main.xml содержит следующую разметку:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Весь интерфейс представлен элементом-контейнером androidx.constraintlayout.widget.ConstraintLayout:

```java
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
```

ConstraintLayout позволяет расположить вложенные элементы в определенных местах экрана. Вначале элемента ConstraintLayout идет определение пространств имен XML:

```java
xmlns:android="http://schemas.android.com/apk/res/android"
xmlns:app="http://schemas.android.com/apk/res-auto"
xmlns:tools="http://schemas.android.com/tools"
```

Каждое пространство имен задается следующим образом: xmlns:префикс="название_ресурса". Например, в

```java
xmlns:android="http://schemas.android.com/apk/res/android"
```

Название ресурса (или URI - Uniform Resource Indicator) - "http://schemas.android.com/apk/res/android". И этот ресурс сопоставляется с префиксом android (xmlns:android).

Зачем эти пространства имен нужны? Каждый ресурс или URI определяет некоторую функциональность, которая используется в приложении, например, предоставляют теги и атрибуты, которые необходимые для построения приложения.

  -  xmlns:android="http://schemas.android.com/apk/res/android": содержит основные атрибуты, которые предоставляются платформой Android, применяются в элементах управления и определяют их визуальные свойства (например, размер, позиционирование)

  -  xmlns:app="http://schemas.android.com/apk/res-auto": содержит атрибуты, которые определены в рамках приложения

  -  xmlns:tools="http://schemas.android.com/tools": применяется для работы с режиме дизайнера в Android Studio

И чтобы упростить работу с этими ресурсами, применяются префиксы. Например, дальше мы видим:

```java
android:layout_width="match_parent"
android:layout_height="match_parent"
tools:context=".MainActivity">
```

android:layout_width определяет ширину контейнера. Этот атрибут (layout_width) расположен в ресурсе "http://schemas.android.com/apk/res/android". И поскольку этот ресурс сопоставляется с префиксом android, то для обращения к атрибуту перед ним через двоеточие указывается префикс данного ресурса.

Значением атрибута android:layout_width является "match_parent". Это значит, что элемент (ConstraintLayout) будет растягиваться по всей ширине контейнера (экрана устройства).

Атрибут android:layout_height="match_parent" определяет высоту контейнера и также определен в "http://schemas.android.com/apk/res/android". Значение "match_parent" указывает, что ConstraintLayout будет растягивается по всей длине контейнера (экрана устройства).

Атрибут tools:context определяет, какой класс activity (экрана приложения) связан с текущим определением интерфейса. В данном случае это класс MainActivity. Это позволяет использовать в Android Studio различные возможности в режиме дизайнера, которые зависят от класса activity.

### TextView

Текстовое поле устанавливает текст с помощью атрибута android:text

```java
<TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
```

   - android:layout_width устанавливает ширину виджета. Значение wrap_content задает для виджета величину, достаточную для отображения в контейнере.

   - android:layout_height устанавливает высоту виджета. Значение wrap_content аналогично установке ширины задает для виджета высоту, достаточную для отображения в контейнере

   - android:text устанавливает текст, который будет выводиться в TextView (в данном случае это строка "Hello World!")

   - app:layout_constraintLeft_toLeftOf="parent": указывает, что левая граница элемента будет выравниваться по левой стороне контейнера ConstraintLayout

   - Обратите внимание, что этот атрибут определен в пространстве имен с префиксом app, то есть в "http://schemas.android.com/apk/res-auto".

   - app:layout_constraintTop_toTopOf="parent": указывает, что верхняя граница элемента будет выравниваться по верхней стороне контейнера ConstraintLayout

   - app:layout_constraintRight_toRightOf="parent": указывает, что правая граница элемента будет выравниваться по правой стороне контейнера ConstraintLayout

   - app:layout_constraintBottom_toBottomOf="parent": указывает, что нижняя граница элемента будет выравниваться по нижней стороне контейнера ConstraintLayout

Стоит отметить, что последние четыре атрибута вместе будут приводить к расположению TextView по центру экрана.

Таким образом, при запуске приложения сначала запускается класс MainActivity, который в качестве графического интерфейса устанавливает разметку из файла activity_main.xml. И поскольку в этой разметке прописан элемент TextView, который представляет некоторый текст, то мы и увидим его текст на экране смартфона.

# Глава 2. Основы создания интерфейса

## 2.1 Java и Android | Создание интерфейса в коде java

### Введение в создание интерфейса

Графический интерфейс пользователя представляет собой иерархию объектов android.view.View и android.view.ViewGroup. Каждый объект ViewGroup представляет контейнер, который содержит и упорядочивает дочерние объекты View. В частности, к контейнерам относят такие элементы, как RelativeLayout, LinearLayout, GridLayout, ConstraintLayout и ряд других.

Простые объекты View представляют собой элементы управления и прочие виджеты, например, кнопки, текстовые поля и т.д., через которые пользователь взаимодействует с программой.

Большинство визуальных элементов, наследующихся от класса View, такие как кнопки, текстовые поля и другие, располагаются в пакете android.widget

При определении визуального у нас есть три стратегии:

  -  Создать элементы управления программно в коде java

  -  Объявить элементы интерфейса в XML

  -  Сочетание обоих способов - базовые элементы разметки определить в XML, а остальные добавлять во время выполнения

Сначала рассмотрим первую стратегию - определение интерейса в коде Java.

Для работы с визуальными элементами создадим новый проект. В качестве шаблона проекта выберем Empty Views Activity.

Пусть новый проект будет называться ViewsApp.

И после создания проекта два основных файла, которые будут нас интересовать при создании визуального интерфейса - это класс MainActivity и определение интерфейса для этой activity в файле activity_main.xml.

MainActivity и activity_main.xml в Android Studio

Определим в классе MainActivity простейший интерфейс:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
 
        // создание TextView
        TextView textView = new TextView(this);
        // установка текста в TextView
        textView.setText("Hello METANIT.COM!");
        // установка высоты текста
        textView.setTextSize(28);
        // установка визуального интерфейса для activity
        setContentView(textView);
    }
}
```

При создании виджетов в коде Java применяется их конструктор, в который передается контекст данного виджета, а точнее объект android.content.Context, в качестве которого выступает текущий класс MainActivity.

```java
TextView textView = new TextView(this);
```

Здесь весь интерфейс представлен элементом TextView, которое предназначено для выводa текста. С помощью методов, которые, как правило, начинаются на set, можно установить различные свойства TextView. Например, в данном случае метод setText() устанавливает текст в поле, а setTextSize() задает высоту шрифта.

Для установки элемента в качестве интерфейса приложения в коде Activity вызывается метод setContentView(), в который передается визуальный элемент.

Если мы запустим приложение, то получим следующий визуальный интерфейс.

Подобным образом мы можем создавать более сложные интерейсы. Например, TextView, вложенный в ConstraintLayout.

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import androidx.constraintlayout.widget.ConstraintLayout;
 
import android.os.Bundle;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
 
        ConstraintLayout constraintLayout = new ConstraintLayout(this);
        TextView textView = new TextView(this);
        textView.setText("Hello METANIT.COM!");
        textView.setTextSize(28);
        // устанавливаем параметры размеров и расположение элемента
        ConstraintLayout.LayoutParams layoutParams = new ConstraintLayout.LayoutParams
                (ConstraintLayout.LayoutParams.WRAP_CONTENT, ConstraintLayout.LayoutParams.WRAP_CONTENT);
        // выравнивание по левому краю ConstraintLayout
        layoutParams.leftToLeft = ConstraintLayout.LayoutParams.PARENT_ID;
        // выравнивание по верхней границе ConstraintLayout
        layoutParams.topToTop = ConstraintLayout.LayoutParams.PARENT_ID;
        // устанавливаем параметры для textView
        textView.setLayoutParams(layoutParams);
        // добавляем TextView в ConstraintLayout
        constraintLayout.addView(textView);
        // в качестве корневого
        setContentView(constraintLayout);
    }
}
```

Для каждого контейнера конкретные действия по добавлению и позиционированию в нем элемента могут отличаться. В данном случае контейнеров выступает класс ConstraintLayout, поэтому для определения позиционирования и размеров элемента необходимо создать объект ConstraintLayout.LayoutParams. (Для LinearLayout это соответственно будет LinearLayout.LayoutParams, а для RelativeLayout - RelativeLayout.LayoutParams и т.д.). Этот объект инициализируется двумя параметрами: шириной и высотой. Для указания ширины и высоты можно использовать константу ViewGroup.LayoutParams.WRAP_CONTENT, которая устанавливает размеры элемента, необходимые для размещения а экране его содержимого.

Далее определяется позиционирование. В зависимости от типа контейнера набор устанавливаемых свойств может отличаться. Так, строка кода

```java
layoutParams.leftToLeft = ConstraintLayout.LayoutParams.PARENT_ID;
```

указывает, что левая граница элемента будет выравниваться по левой ганице контейнера.

А строка кода

```java
layoutParams.topToTop = ConstraintLayout.LayoutParams.PARENT_ID;
```

указывает, что верхняя граница элемента будет выравниваться по верхней ганице контейнера. В итоге элемент будет размещен в левом верхнем углу ConstraintLayout.

Для установки всех этих значений для конкретного элемента (TextView) в его метод setLayoutParams() передается объект ViewGroup.LayoutParams (или один из его наследников, например, ConstraintLayout.LayoutParams).

```java
textView.setLayoutParams(layoutParams);
```

Все классы контейнеров, которые наследуются от android.view.ViewGroup (RelativeLayout, LinearLayout, GridLayout, ConstraintLayout и т.д.), имеют метод void addView(android.view.View child), который позволяет добавить в контейнер другой элемент - обычный виджет типа TextView или другой контейнер. И в данном случае посредством данного метода TextView добавляется в ConstraintLayout:

```java
constraintLayout.addView(textView);
```

Опять же отмечу, что для конкретного контейнера конкретные действия могут отличаться, но как правило для всех характерно три этапа:

  -  Создание объекта ViewGroup.LayoutParams и установка его свойств

  -  Передача объекта ViewGroup.LayoutParams в метод setLayoutParams() элемента

  -  Передача элемента для добавления в метод addView() объекта контейнера

Хотя мы можем использовать подобный подход, в то же время более оптимально определять визуальный интерейс в файлах xml, а всю связанную логику определять в классе activity. Тем самым мы достигнем разграничения интерфейса и логики приложения, их легче будет разрабатывать и впоследствии модифицировать. И в следующей теме мы это рассмотрим.

## 2.2 Java и Android | Определение интерфейса в файле XML. Файлы layout

Как правило, для определения визуального интерфейса в проектах под Android используются специальные файлы xml. Эти файлы являются ресурсами разметки и хранят определение визуального интерфейса в виде кода XML. Подобный подход напоминает создание веб-сайтов, когда интерфейс определяется в файлах html, а логика приложения - в коде javascript.

Объявление пользовательского интерфейса в файлах XML позволяет отделить интерфейс приложения от кода. Что означает, что мы можем изменять определение интерфейса без изменения кода java. Например, в приложении могут быть определены разметки в файлах XML для различных ориентаций монитора, различных размеров устройств, различных языков и т.д. Кроме того, объявление разметки в XML позволяет легче визуализировать структуру интерфейса и облегчает отладку.

Файлы разметки графического интерфейса располагаются в проекте в каталоге res/layout. По умолчанию при создании проекта с пустой activity уже есть один файл ресурсов разметки activity_main.xml, который может выглядеть примерно так:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

В файле определяются все графические элементы и их атрибуты, которые составляют интерфейс. При создании разметки в XML следует соблюдать некоторые правила: каждый файл разметки должен содержать один корневой элемент, который должен представлять объект View или ViewGroup.

В данном случае корневым элементом является элемент ConstraintLayout, который содержит элемент TextView.

Как правило, корневой элемент содержит определение используемых пространств имен XML. Например, в коде по умолчанию в ConstraintLayout мы можем увидеть такие атрибуты:

Каждое пространство имен задается следующим образом: xmlns:префикс="название_ресурса". Например, в

```java
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
```

Название ресурса (или URI - Uniform Resource Indentifier) - "http://schemas.android.com/apk/res/android". И этот ресурс сопоставляется с префиксом android (xmlns:android). То есть через префикс мы сможем ссылаться на функциональность этого пространства имен.

Каждое пространство имен определяет некоторую функциональность, которая используется в приложении, например, предоставляют теги и атрибуты, которые необходимые для построения приложения.

 - xmlns:android="http://schemas.android.com/apk/res/android": содержит основные атрибуты, которые предоставляются платформой Android, применяются в элементах управления и определяют их визуальные свойства (например, размер, позиционирование). Например, в коде ConstraintLayout используется следующий атрибут из пространства имен "http://schemas.android.com/apk/res/android":

   ```java
    android:layout_width="match_parent"
   ```

- xmlns:app="http://schemas.android.com/apk/res-auto": содержит атрибуты, которые определены в рамках приложения. Например, в коде TextView:

  ```java
    app:layout_constraintBottom_toBottomOf="parent"
  ```
- xmlns:tools="http://schemas.android.com/tools": применяется для работы с режиме дизайнера в Android Studio

Это наиболее распространенные пространства имен. И обычно каждый корневой элемент (не обязательно только ConstraintLayout) их содержит. Однако, если вы не планируете пользоваться графическим дизайнером в Android Studio и хотите работать целиком в коде xml, то соответственно смысла в пространстве имен "http://schemas.android.com/tools" нет, и его можно убрать.

При компиляции каждый XML-файл разметки компилируется в ресурс View. Загрузка ресурса разметки осуществляется в методе Activity.onCreate. Чтобы установить разметку для текущего объекта activity, надо в метод setContentView() в качестве параметра передать ссылку на ресурс разметки.

```java
  setContentView(R.layout.activity_main);
```

Для получения ссылки на ресурс в коде java необходимо использовать выражение R.layout.[название_ресурса]. Название ресурса layout будет совпадать с именем файла, поэтому чтобы использовать файл activity_main.xml в качестве источника визуального интерфейса, можно определить следующий код в классе MainActivity:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
         
        // загрузка интерфейса из файла activity_main.xml
        setContentView(R.layout.activity_main);
    }
}
```

### Добавление файла layout

Но у нас может быть и несколько различных ресурсов layout. Как правило, каждый отдельный класс Activity использует свой файл layout. Либо для одного класса Activity может использоваться сразу несколько различных файлов layout.

К примеру, добавим в проект новый файл разметки интерфейса. Для этого нажмем на папку res/layout правой кнопкой мыши и в появившемся меню выберем пункт New -> Layout Resource File:

После этого в специальном окошке будет предложено указать имя и корневой элемент для файла layout:

В качестве названия укажем second_layout. Все остальные настройки оставим по умолчанию:

 -   в поле Root element указывается корневой элемент. По умолчанию это androidx.constraintlayout.widget.ConstraintLayout.

 -   поле Source set указывает, куда помещать новый файл. По умолчанию это main - область проекта, с которой мы собственно работаем при разаботке приложения.

 -   поле Directory main указывает папку в рамках каталога, выбранного в предыдущей опции, в который собственно помещается новый файл. По умолчанию для файлов с разметкой интерфейса это layout.

После этого в папку res/layout будет добавлен новый файл second_layout.xml, с которым мы можем работать точно также, как и с activity_main.xml. В частности, откроем файл second_layout.xml и изменим его содержимое следующим образом:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
 
    <TextView
        android:id="@+id/header"
        android:text="Welcome to Android"
        android:textSize="26sp"
        android:layout_width="match_parent"
        android:layout_height="match_parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Здесь определено текстовое поле TextView, которое имеет следующие атрибуты:



-    android:id - идентификатор элемента, через который мы сможем ссылаться на него в коде. В записи android:id="@+id/header" символ @ указывает XML-парсеру использовать оставшуюся часть строки атрибута как идентификатор. А знак + означает, что если для элемента не определен id со значением header, то его следует определить.

-    android:text - текст элемента - на экран будет выводиться строка "Welcome to Android".

-    android:textSize - высота шрифта (здесь 26 единиц)

-    android:layout_width - ширина элемента. Значение "match_parent" указывает, что элемент будет растягиваться по всей ширине контейнера ConstraintLayout

-    android:layout_height - высота элемента. Значение "match_parent" указывает, что элемент будет растягиваться по всей высоте контейнера ConstraintLayout

Применим этот файл в качестве определения графического интерфейса в классе MainActivity:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.second_layout);
    }
}
```

Файл интерфейса называется second_layout.xml, поэтому по умолчанию для него будет создаваться ресурс R.layout.second_layout. Соответственно, чтобы его использовать, мы передаем его в метода setContentView. В итоге мы увидим на экране следующее:

### Получение и управлене визуальными элементами в коде

Выше определенный элемент TextView имеет один очень важный атрибут - id или идентификатор элемента. Этот идентификатор позволяет обращаться к элементу, который определен в файле xml, из кода Java. Например, перейдем к классу MainActivity и изменим его код:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        // устанавливаем в качестве интерфейса файл second_layout.xml
        setContentView(R.layout.second_layout);
 
        // получаем элемент textView
        TextView textView = findViewById(R.id.header);
        // переустанавливаем у него текст
        textView.setText("Hello from Java!");
    }
}
```

С помощью метода setContentView() устанавливается разметка из файла second_layout.xml.

Другой важный момент, который стоит отметить - получение визуального элемента TextView. Так как в его коде мы определили атрибут android:id, то через этот id мы можем его получить.

Для получения элементов по id класс Activity имеет метод findViewById(). В этот метод передается идентификатор ресурса в виде R.id.[идентификатор_элемента]. Этот метод возвращает объект View - объект базового класса для всех элементов, поэтому результат метода еще необходимо привести к типу TextView.

Далее мы можем что-то сделать с этим элементом, в данном случае изменяем его текст.

Причем что важно, получение элемента происходит после того, как в методе setContentView была установлена разметка, в которой этот визуальный элемент был определен.

И если мы запустим проект, то увидим, что TextView выводит новый текст.

## 2.3 Java и Android | Определение размеров

### Определение размеров

При разработке приложений под Android мы можем использовать различные типы измерений:

-    px: пиксели текущего экрана. Однако эта единица измерения не рекомендуется, так как реальное представление внешнего вида может изменяться в зависимости от устройства; каждое устройство имеет определенный набор пикселей на дюйм, поэтому количество пикселей на экране может также меняться

-    dp: (density-independent pixels) независимые от плотности экрана пиксели. Абстрактная единица измерения, основанная на физической плотности экрана с разрешением 160 dpi (точек на дюйм). В этом случае 1dp = 1px. Если размер экрана больше или меньше, чем 160dpi, количество пикселей, которые применяются для отрисовки 1dp соответственно увеличивается или уменьшается. Например, на экране с 240 dpi 1dp=1,5px, а на экране с 320dpi 1dp=2px. Общая формула для получения количества физических пикселей из dp: px = dp * (dpi / 160)

-    sp: (scale-independent pixels) независимые от масштабирования пиксели. Допускают настройку размеров, производимую пользователем. Рекомендуются для работы со шрифтами.

-    pt: 1/72 дюйма, базируются на физических размерах экрана

-    mm: миллиметры

-    in: дюймы

Предпочтительными единицами для использования являются dp. Это связано с тем, что мир мобильных устройств на Android сильно фрагментирован в плане разрешения и размеров экрана. И чем больше плотность пикселей на дюйм, тем соответственно больше пикселей нам будет доступно:

Используя же стандартные физические пиксели мы можем столкнуться с проблемой, что размеры элементов также будут сильно варьироваться в зависимости от плотности пикселей устройства. Например, возьмем 3 устройства с различными характеристиками экрана Nexus 4, Nexus 5X и Nexus 6P и выведем на экран квадрат размером 300px на 300px:

В одном случае квадрат по ширине будет занимать 40%, в другом - треть ширины, в третьем - 20%.

Теперь также возьмем квадрат со сторонами 300х300, но теперь вместо физических пикселей используем единицы dp:

Теперь же размеры квадрата на разных устройствах выглядят более консистентно.

Для упрощения работы с размерами все размеры разбиты на несколько групп:

-    ldpi (low): ~120dpi

-    mdpi (medium): ~160dpi

-    hdpi (high): ~240dpi (к данной группе можно отнести такое древнее устройство как Nexus One)

-    xhdpi (extra-high): ~320dpi (Nexus 4)

-    xxhdpi (extra-extra-high): ~480dpi (Nexus 5/5X, Samsung Galaxy S5)

 -   xxxhdpi (extra-extra-extra-high): ~640dpi (Nexus 6/6P, Samsung Galaxy S6)

### Установка размеров

Основная проблема, связанная с размерами, связана с их установкой в коде Java. Например, некоторые методы принимают в качестве значения физические пиксели, а не density-independent pixels. В этом случае может потребоваться перевести значения из одного типа единиц в другой. Для этого требуется применить метод TypedValue.applyDimension(), который принимает три параметра:

```java
public static float applyDimension(int unit,
                                   float value,
                                   android.util.DisplayMetrics metrics)
```

Параметр unit представляет тип единиц, из которой надо получить значение в пикселях. Тип единиц описывается одной из констант TypedValue:

-    COMPLEX_UNIT_DIP - dp или независимые от плотности экрана пиксели

-    COMPLEX_UNIT_IN - in или дюймы

 -   COMPLEX_UNIT_MM - mm или миллиметры

 -   COMPLEX_UNIT_PT - pt или точки

 -   COMPLEX_UNIT_PX - px или физические пиксели

 -  COMPLEX_UNIT_SP - sp или независимые от масштабирования пиксели (scale-independent pixels)

Параметр value представляет значение, которое надо преобразовать.

Параметр metrics представляет информацию о метрике, в рамках коорой надо выполнить преобразование.

В итоге метод возвращает преобразованное значение. Рассмотрим абстрактный пример. Например, нам надо получить из 60dp обычные физические пиксели:

```java
int valueInDp = 60;
int valueInPx = (int) TypedValue.applyDimension(
                TypedValue.COMPLEX_UNIT_DIP, valueInDp, getResources().getDisplayMetrics());
```

В качестве третьго аргумента передается вызов метода getResources().getDisplayMetrics(), который позволяет получить информацию о метрике, связанной с текущим устройством. В итоге мы получим из 60dp некоторое количество пикселей.

## 2.4 Java и Android | Ширина и высота элементов

### Ширина и высота элементов

Все визуальные элеметы, которые мы используем в приложении, как правило, упорядочиваются на экране с помощью контейнеров. В Android подобными контейнерами служат такие классы как RelativeLayout, LinearLayout, GridLayout, TableLayout, ConstraintLayout, FrameLayout. Все они по разному располагают элементы и управляют ими, но есть некоторые общие моменты при компоновке визуальных компонентов, которые мы сейчас рассмотрим.

Для организации элементов внутри контейнера используются параметры разметки. Для их задания в файле xml используются атрибуты, которые начинаются с префикса layout_. В частности, к таким параметрам относятся атрибуты layout_height и layout_width, которые используются для установки размеров и могут использовать одну из следующих опций:

-    Растяжение по всей ширине или высоте контейнера с помощью значения match_parent (для всех контейнеров кроме ConstraintLayout) или 0dp (для ConstraintLayout)

-    Растяжение элемента до тех границ, которые достаточны, чтобы вместить все его содержимое с помощью значения wrap_content

-    Точные размеры элемента, например 96 dp

### match_parent

Установка значения match_parent позволяет растянуть элемент по всей ширине или высоте контейнера. Стоит отметить, что данное значение применяется ко всем контейнерам, кроме ConstraintLayout. Например, рястянем элемент TextView по всей ширине и высоте контейнера LinearLayout:

```java
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
 
    <TextView
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:text="Hello World!"
        android:textSize="30sp"
        android:background="#e0e0e0" />
     
</LinearLayout>
```

Контейнер самого верхнего уровня, в качестве которого в данном случае выступает LinearLayout, для высоты и ширины имеет значение match_parent, то есть он будет заполнять всю область для activity - как правило, весь экран.

И TextView также принимает подобные атрибуты. Значение android:layout_width="match_parent" обеспечивает растяжение по ширине, а android:layout_height="match_parent" - по вертикали. Для наглядности в TextView применяет атрибут android:background, который представляет фон и в данном случае окрашивает элемент в цвет "#e0e0e0", благодаря чему мы можем увидеть занимаемую им область.

Следует учитывать, что значение match_parent можно применять почти во всех встроенных контейнерах, типа LinearLayout или RelativeLayout и их элементах. Однако match_parent не рекомендуется применять к элементам внутри ConstraintLayout. Вместо "match_parent" в ConstraintLayout можно использовать значение 0dp, чтобы растянуть элемент по горизонтали или вертикали:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <TextView
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:text="Hello World!"
        android:textSize="30sp"
        android:background="#e0e0e0"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintBottom_toBottomOf="parent"
        />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Стоит отметить, что ConstraintLayout сама также растягивается по ширине и высоте экрана с помощью значения "match_parent" в атрибутах layout_width и android:layout_height, но к вложенным элементам это значение не рекомендуется применять.

Поскольку ConstraintLayout имеет некоторые особенности при установке размеров, то более подробно работа с размерами элементов именно в ConstraintLayout раскрыта более подробно в одной из следующих тем.

### wrap_content

Значение wrap_content устанавливает те значения для ширины или высоты, которые необходимы, чтобы разместить на экране содержимое элемента:

```java<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        android:textSize="30sp"
        android:background="#ffcdd2"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
    />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Здесь элемент TextView растягивается до тех значений, которые достаточны для размещения его текста.

### Установка точных значений

Также мы можем установить точные значения:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <TextView
        android:layout_height="90dp"
        android:layout_width="150dp"
        android:text="Hello World!"
        android:textSize="30sp"
        android:background="#e0e0e0"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Кроме того, можно комбинировать несколько значений, например, растянуть по ширине содержимого и установить точные значения для высоты:

```java
<TextView
        android:layout_height="80dp"
        android:layout_width="wrap_content"
        android:text="Hello World!"
        android:textSize="30sp"
        android:background="#e0e0e0"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
/>
```

Если для установки ширины и длины используется значение wrap_content, то мы можем дополнительно ограничить минимальные и максимальные значения с помощью атрибутов minWidth/maxWidth и minHeight/maxHeight:

```java
<TextView
        android:minWidth="200dp"
        android:maxWidth="250dp"
        android:minHeight="100dp"
        android:maxHeight="200dp"
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:text="Hello World!"
        android:textSize="30sp"
        android:background="#e0e0e0"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
/>
```

В этом случае ширина TextView будет такой, которая достаточна для вмещения текста, но не больше значения maxWidth и не меньше значения minWidth. То же самое для установки высоты.

### Программная установка ширины и высоты

Если элемент, к примеру, тот же TextView создается в коде java, то для установки высоты и ширины можно использовать метод setLayoutParams(). Так, изменим код MainActivity:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import androidx.constraintlayout.widget.ConstraintLayout;
import android.os.Bundle;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
 
        ConstraintLayout constraintLayout = new ConstraintLayout(this);
        TextView textView = new TextView(this);
        textView.setText("Hello Android");
        textView.setTextSize(26);
 
        // устанавливаем параметры размеров и расположение элемента
        ConstraintLayout.LayoutParams layoutParams = new ConstraintLayout.LayoutParams
                (ConstraintLayout.LayoutParams.WRAP_CONTENT, ConstraintLayout.LayoutParams.WRAP_CONTENT);
        // эквивалент app:layout_constraintLeft_toLeftOf="parent"
        layoutParams.leftToLeft = ConstraintLayout.LayoutParams.PARENT_ID;
        // эквивалент app:layout_constraintTop_toTopOf="parent"
        layoutParams.topToTop = ConstraintLayout.LayoutParams.PARENT_ID;
        // устанавливаем параметры для textView
        textView.setLayoutParams(layoutParams);
        // добавляем TextView в ConstraintLayout
        constraintLayout.addView(textView);
        setContentView(constraintLayout);
    }
}
```

В метод setLayoutParams() передается объект ViewGroup.LayoutParams. Этот объект инициализируется двумя параметрами: шириной и высотой. Для указания ширины и высоты можно использовать одну из констант ViewGroup.LayoutParams.WRAP_CONTENT или ViewGroup.LayoutParams.MATCH_PARENT (в случае с LinearLayout или RelativeLayout).

Поскольку в данном случае мы имеем дело с контейнером ConstraintLayout, то для установки размеров применяется значение ConstraintLayout.LayoutParams.WRAP_CONTENT. В реальности класс androidx.constraintlayout.widget.ConstraintLayout.LayoutParams, который предоставляет это значение, наследуется от android.view.ViewGroup.LayoutParams

Также мы можем передать точные значения или комбинировать типы значений:

```java
ConstraintLayout.LayoutParams layoutParams = new ConstraintLayout.LayoutParams
                (ConstraintLayout.LayoutParams.WRAP_CONTENT, 200);
```

## 2.5 Java и Android | Внутренние и внешние отступы

### Внутренние и внешние отступы

Параметры разметки позволяют задать отступы как от внешних границ элемента до границ контейнера, так и внутри самого элемента между его границами и содержимым.

### Padding

Для установки внутренних отступов применяется атрибут android:padding. Он устанавливает отступы контента от всех четырех сторон контейнера. Можно устанавливать отступы только от одной стороны контейнера, применяя следующие атрибуты: android:paddingLeft, android:paddingRight, android:paddingTop и android:paddingBottom.

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="50dp"
    tools:context=".MainActivity">
 
    <TextView
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:text="Hello World!"
        android:textSize="30sp"
        android:background="#e0e0e0"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
    />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

У контейнера ConstraintLayout установлен только один общий внутренний отступ в 50 единиц. Вложенный элемент TextView позиционируется в левом верхнем углу контейнера (благодаря атрибутам app:layout_constraintLeft_toLeftOf="parent" и app:layout_constraintTop_toTopOf="parent"). . Поэтому TextView будет отодвигаться от начальной точки (левый верхний угол контейнера ConstraintLayout) вниз и влево на 50 единиц. Кроме того, такие же отступы будут действовать справа и снизу, если элемент будет примыкать к нижней или правой границе контейнера.

Установка одного отступа

```java
android:padding="50dp"
```

Будет аналогична установке четырех отступов

```java
android:paddingTop="50dp"
android:paddingLeft="50dp"
android:paddingBottom="50dp"
android:paddingRight="50dp"
```

Подобным образом можно установить отступы в других элементах. Например, установим внутри TextView сверху и снизу от внутреннего содержимого (то есть текста) отступы в 60 единиц и отступы слева и справа в 40 единиц:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="50dp"
    tools:context=".MainActivity">
 
    <TextView
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:paddingTop="60dp"
        android:paddingLeft="40dp"
        android:paddingRight="40dp"
        android:paddingBottom="60dp"
        android:text="Hello World!"
        android:textSize="30sp"
        android:background="#e0e0e0"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Стоит отметить, что вместо атрибутов android:paddingLeft и android:paddingRight можно применять атрибуты android:paddingStart и android:paddingEnd, которые разработаны специально адаптации приложения для работы как для языков с левосторонней ориентацией, так и правосторонней ориентацией (арабский, фарси).

### Margin

Для установки внешних отступов используется атрибут layout_margin. Данный атрибут имеет модификации, которые позволяют задать отступ только от одной стороны: android:layout_marginBottom, android:layout_marginTop, android:layout_marginLeft и android:layout_marginRight (отступы соответственно от нижней, верхней, левой и правой границ):

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <TextView
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:layout_marginTop="50dp"
        android:layout_marginLeft="60dp"
        android:text="Hello World!"
        android:textSize="30sp"
        android:background="#e0e0e0"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
    />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Здесь у TextView задаются отступы от двух сторон ConstraintLayout (слева 60 единиц и сверху 50 единиц):

### Программная установка отступов

Для программной установки внутренних отступов у элементы вызывается метод setPadding(left, top, right, bottom), в который передаются четыре значения для каждой из сторон. Также можно по отдельности задать отступы с помощью методов getPaddingLeft(), getPaddingTop(), getPaddingRight() и getPaddingBottom().

Для установки внешних отступов необходимо реализовать объект LayoutParams для того контейнера, который применяется. И затем вызвать у этого объекта LayoutParams метод setMargins(left, top, right, bottom):

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import androidx.constraintlayout.widget.ConstraintLayout;
 
import android.os.Bundle;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
 
        ConstraintLayout constraintLayout = new ConstraintLayout(this);
        TextView textView = new TextView(this);
        // установка цвета текстового поля
        textView.setBackgroundColor(0xFFE0E0E0);
        // установка текста текстового поля
        textView.setText("Hello Android");
        // установка размера текста
        textView.setTextSize(30);
 
        ConstraintLayout.LayoutParams layoutParams = new ConstraintLayout.LayoutParams
                (ConstraintLayout.LayoutParams.WRAP_CONTENT , ConstraintLayout.LayoutParams.WRAP_CONTENT);
        // установка внешних отступов
        layoutParams.setMargins(60, 50, 60, 50);
        // позиционирование в левом верхнем угду контейнера
        // эквивалент app:layout_constraintLeft_toLeftOf="parent"
        layoutParams.leftToLeft = ConstraintLayout.LayoutParams.PARENT_ID;
        // эквивалент app:layout_constraintTop_toTopOf="parent"
        layoutParams.topToTop = ConstraintLayout.LayoutParams.PARENT_ID;
        // устанавливаем размеры
        textView.setLayoutParams(layoutParams);
        // установка внутренних отступов
        textView.setPadding(40,40,40,40);
        // добавляем TextView в ConstraintLayout
        constraintLayout.addView(textView);
 
        setContentView(constraintLayout);
    }
}
```

Поскольку в данном случае элемент TextView добавляется в контейнер типа ConstraintLayout, то для его позиционирования применяется объект ConstraintLayout.LayoutParams (соответственно для LinearLayout это будет LinearLayout.LayoutParams), у которого вызывается метод setMargins().

Но если посмотреть на последний скриншот, то можно увидеть, что, несмотря на то, что отступы вроде бы заданы также, что и в предпоследнем примере в файле layout, однако в реальности на экране мы увидим отступы со совсем другими значениями. Дело в том, что методы setPadding() и setMargins() принимают значения в пикселях, тогда как в файле layout применялись единицы dp. И чтобы использовать dp также в коде, необходимо выполнить преобразования:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import androidx.constraintlayout.widget.ConstraintLayout;
 
import android.os.Bundle;
import android.util.TypedValue;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
 
        ConstraintLayout constraintLayout = new ConstraintLayout(this);
        TextView textView = new TextView(this);
        textView.setBackgroundColor(0xFFE0E0E0);
        textView.setText("Hello Android!");
        textView.setTextSize(30);
 
        // получаем отступ в пикселях для 50 dp
        int margin50inDp = (int) TypedValue.applyDimension(
                TypedValue.COMPLEX_UNIT_DIP, 50, getResources().getDisplayMetrics());
        // получаем отступ в пикселях для 60 dp
        int margin60inDp = (int) TypedValue.applyDimension(
                TypedValue.COMPLEX_UNIT_DIP, 60, getResources().getDisplayMetrics());
        // получаем отступ в пикселях для 40 dp
        int padding40inDp = (int) TypedValue.applyDimension(
                TypedValue.COMPLEX_UNIT_DIP, 40, getResources().getDisplayMetrics());
 
        ConstraintLayout.LayoutParams layoutParams = new ConstraintLayout.LayoutParams
                (ConstraintLayout.LayoutParams.WRAP_CONTENT , ConstraintLayout.LayoutParams.WRAP_CONTENT);
        // установка внешних отступов
        layoutParams.setMargins(margin60inDp, margin50inDp, margin60inDp, margin50inDp);
        // выравнивание по левому краю ConstraintLayout
        layoutParams.leftToLeft = ConstraintLayout.LayoutParams.PARENT_ID;
        // выравнивание по верхней границе ConstraintLayout
        layoutParams.topToTop = ConstraintLayout.LayoutParams.PARENT_ID;
        // устанавливаем размеры
        textView.setLayoutParams(layoutParams);
        // установка внутренних отступов
        textView.setPadding(padding40inDp, padding40inDp, padding40inDp, padding40inDp);
        // добавляем TextView в ConstraintLayout
        constraintLayout.addView(textView);
 
        setContentView(constraintLayout);
    }
}
```

## 2.6
