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

## 2.6 Java и Android | ConstraintLayout

ConstraintLayout представляет контейнер, который позволяет создавать гибкие и масштабируемые визуальные интерфейсы.

Для позиционирования элемента внутри ConstraintLayout необходимо указать ограничения (constraints). Есть несколько типов ограничений. В частности, для установки позиции относительно определенного элемента испльзуются следующие ограничения:

-    layout_constraintLeft_toLeftOf: левая граница позиционируется относительно левой границы другого элемента

-    layout_constraintLeft_toRightOf: левая граница позиционируется относительно правой границы другого элемента

-    layout_constraintRight_toLeftOf: правая граница позиционируется относительно левой границы другого элемента

-    layout_constraintRight_toRightOf: правая граница позиционируется относительно правой границы другого элемента

-    layout_constraintTop_toTopOf: верхняя граница позиционируется относительно верхней границы другого элемента

-    layout_constraintTop_toBottomOf: верхняя граница позиционируется относительно нижней границы другого элемента

-    layout_constraintBottom_toBottomOf: нижняя граница позиционируется относительно нижней границы другого элемента

-    layout_constraintBottom_toTopOf: нижняя граница позиционируется относительно верхней границы другого элемента

-    layout_constraintBaseline_toBaselineOf: базовая линия позиционируется относительно базовой линии другого элемента

-    layout_constraintStart_toEndOf: элемент начинается там, где завершается другой элемент

-    layout_constraintStart_toStartOf: элемент начинается там, где начинается другой элемент

-    layout_constraintEnd_toStartOf: элемент завершается там, где начинается другой элемент

-    layout_constraintEnd_toEndOf: элемент завершается там, где завершается другой элемент

Возможно, по поводу четырех последних свойств возникло некоторое непонимание, что подразумевается под началом или завершением элемента. Дело в том, что некоторые языки (например, арабский или фарси) имеют правостороннюю ориентацию, то есть символы идут справа налево, а не слева направо, как в европейских языках. И в зависимости от текущей ориентации - левосторонняя или правосторонняя - будет изменяться то, где именно начало, а где завершение элемента. Например, при левосторонней ориентации начало - слева, а завершение - справа, поэтому атрибут layout_constraintStart_toEndOf фактически будет аналогичен атрибуту layout_constraintLeft_toRightOf. А при правосторонней ориентации - атрибуту layout_constraintRight_toLeftOf, так как начало справа, а завершение - слева

Каждое ограничение устанавливает позиционирование элемента либо по горизонтали, либо по вертикали. И для определения позиции элемента в ConstraintLayout необходимо указать как минимум одно ограничение по горизонтали и одно ограничение по вертикали.

Позиционирования может производиться относительно границ самого контейнера ContentLayout (в этом случае ограничение имеет значение parent), либо же относительно любого другого элемента внутри ConstraintLayout, тогда в качестве значения ограничения указывается id этого элемента.

Простейший пример:

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
        android:textSize="30sp"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

В данном случае у элемента TextView установлено два ограничение: одно погоризонтальной линии (app:layout_constraintLeft_toLeftOf="parent"), второе - по вертикальной линии (app:layout_constraintTop_toTopOf="parent"). Оба ограничения устанавливаются относительно контейнера ConstraintLayout, поэтому они принимают значение parent, то есть ConstraintLayout.

Ограничение app:layout_constraintLeft_toLeftOf="parent" устанавливает левую границу TextView у левой границы контейнера.

Ограничение app:layout_constraintTop_toTopOf="parent" устанавливает верхнюю границу TextView у верхней границы контейнера.

В итоге TextView будет располагаться в верхнем левом углу контейнера.

Стоит обратить внимание, что все эти атрибуты ограничений берутся из пространства имен "http://schemas.android.com/apk/res-auto", которое проецируется на префикс app.

Если необходимо установить ограничение относительно другого элемента, то необходимо указать id этого элемента:

```java
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <EditText
        android:id="@+id/editText"
        android:layout_width="180dp"
        android:layout_height="wrap_content"
        android:hint="Введите Email"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Отправить"
        app:layout_constraintLeft_toRightOf="@id/editText"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Здесь для текстового поля ввода EditText устанавливаются два ограничения относительно родительского контейнера ConstraintLayout, поэтому ограничения имеют значение parent, а сам EditText выравнивается по левой и верхней границе контейнера. Верхняя граница кнопки Button также выравнивается по верхней границе контейнера. А вот левая граница кнопки выравнивается по правой границе EditText. Для этого в качестве значения атрибута передается id EditText:

```java
app:layout_constraintLeft_toRightOf="@id/editText"
```

Подобным образом можно составлять различные комбинации атрибутов для определения нужного нам позиционирования. Например, изменим код кнопки:

```java
<Button
    android:id="@+id/button"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Отправить"
    app:layout_constraintLeft_toRightOf="@id/editText"
    app:layout_constraintTop_toBottomOf="@id/editText" />
```

В данном случае верхняя граница кнопки выравнивается по нижней границе EditText

Более того мы можем позиционировать оба элемента один относительно другого:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <EditText
        android:id="@+id/editText"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:hint="Введите Email"
        app:layout_constraintRight_toLeftOf="@+id/button"
        app:layout_constraintTop_toTopOf="parent" />
    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Отправить"
        app:layout_constraintLeft_toRightOf="@id/editText"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

### Позиционирование в центре

Если необходимо расположить элемент в центре контейнера по вертикали, то надо использовать пару атрибутов

```java
app:layout_constraintTop_toTopOf="parent"
app:layout_constraintBottom_toBottomOf="parent"
```

Если необходимо расположить элемент в центре контейнера по горизонтали, то надо использовать следующую пару атрибутов

```java
app:layout_constraintLeft_toLeftOf="parent"
app:layout_constraintRight_toRightOf="parent"
```

Соответственно для расположения в центре контейнера по вертикали и горизонтали надо применить все выше указанные четыре атрибута:

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
        android:text="Hello Android"
        android:textSize="30sp"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintBottom_toBottomOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

### Сдвиг

Сдвиг

Если элементы расположены по центру, ConstraintLayout позволяет их сдвигать по горизонтали и по вертикали. Для сдвига по горизонтали применяется атрибут layout_constraintHorizontal_bias, а для сдвига по вертикали - атрибут layout_constraintVertical_bias. В качестве значения они принимают число с плавающей точкой от 0 до 1. Значение по умолчанию - 0.5 (расположение по центру). Например:

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
        android:text="Top TextView"
        android:textSize="30sp"
        android:background="#e0e0e0"
 
        app:layout_constraintHorizontal_bias="0.2"
 
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent"/>
 
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Bottom TextView"
        android:textSize="30sp"
        android:background="#e0e0e0"
 
        app:layout_constraintHorizontal_bias=".9"
 
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintBottom_toBottomOf="parent"/>
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Первый TextView сдвигается на 20% от левой границы контейнера (значение по умолчанию - 0.5, поэтому при значении 0.2 элемент сдвигается влево). Второй TextView сдвигается на 90% от левой границы контейнера. Например, значение 1 означало бы, что элемент придвинут к правой границе, а значение 0 - к левой

Аналогично работает атрибут layout_constraintVertical_bias, который сдвигает по вертикали.

## 2.7 Java и Android | Размеры элементов в ConstraintLayout

В ConstraintLayout применяются три способа установки размеров:

  -  Установка точных размеров, например, 123dp

  - Значение WRAP_CONTENT, которое задает для виджета размеры, достаточные для расположения его содержимого

  - Значение 0dp, которое эквивалентно значению "MATCH_CONSTRAINT" в коде Java. В этом случае размеры элемента устанавливаются исходя из указанных для него ограничений. По умолчанию элемент занимает все доступное пространство.

Применим все три типа установки размеров:

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
        android:layout_width="160dp"
        android:layout_height="wrap_content"
        android:text="Top TextView"
        android:textSize="30sp"
        android:background="#e0e0e0"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent"/>
 
    <TextView
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:text="Center TextView"
        android:textSize="30sp"
        android:background="#e0e0e0"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintBottom_toBottomOf="parent"/>
 
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Bottom TextView"
        android:textSize="30sp"
        android:background="#e0e0e0"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintBottom_toBottomOf="parent"/>
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Здесь создаются три элемента TextView. Все они центрируются по горизонтали, но по вертикали располагаются по верхней и нижней границе контейнера и в центре. Для всех трех TextView для высоты задано значение wrap_content, то есть все три элемента будут занимать ту высоту, которая для них предпочтительна, чтобы вместить содержимое:

```java
android:layout_height="wrap_content"
```

Однако для каждого элемента заданы свои настройки ширины. Для верхнего TextView установлены точные размеры - 160 единиц:

```java
android:layout_width="160dp"
```

Для центрального TextView установлено значение "0dp", благодаря чему элемент по умолчанию будет занимать все доступное для него пространство (в данном случае растягиваться по горизонтали):

```java
android:layout_width="0dp"
```

Для нижнего TextView установлено значение "wrap_content", то есть элемент будет принимать ту ширину, которая необходима для вмещения его содержимого:

```java
android:layout_width="wrap_content"
```

Стоит отметить, что во вложенных виджетах в ConstraintLayout не рекомендуется использовать значение match_parent, которое позволяет виджету занять все доступное пространство. Вместо этого рекомендуется использовать 0dp или "MATCH_CONSTRAINT" - вместе с другими ограничениями они дадут необходимый эффект. Так, для растяжения по ширине контейнера применяются следующие атрибуты:

```java
android:layout_width="0dp"
app:layout_constraintLeft_toLeftOf="parent"
app:layout_constraintRight_toRightOf="parent"
```

А для растяжения по высоте контейнера применяются следующие атрибуты:

```java
android:layout_height="0dp"
app:layout_constraintTop_toTopOf="parent"
app:layout_constraintBottom_toBottomOf="parent"
```

Например, растяжение TextView по всей длине и ширине контейнера:

```java
<TextView
    android:layout_width="0dp"
    android:layout_height="0dp"
    android:text="Hello Android"
    android:textSize="30sp"
    android:background="#e0e0e0"
    app:layout_constraintLeft_toLeftOf="parent"
    app:layout_constraintRight_toRightOf="parent"
    app:layout_constraintTop_toTopOf="parent"
    app:layout_constraintBottom_toBottomOf="parent"/>
```

### Минимальные и максимальные размеры

Ряд атрибутов задают максимальные и минимальные размеры:

 -   layout_constraintWidth_min и layout_constraintHeight_min: представляют соответственно минимальную ширину и высоту

 -   layout_constraintWidth_max и layout_constraintHeight_max: представляют соответственно максимальную ширину и высоту

В качестве значения они принимают точное значение в dp или значение wrap (аналогично wrap_content). Например:

```java
<TextView
    android:layout_width="260dp"
    android:layout_height="wrap_content"
    android:text="Hello Android"
    android:textSize="30sp"
    android:background="#e0e0e0"
 
    app:layout_constraintHeight_max="200dp"
    app:layout_constraintWidth_max="200dp"
    app:layout_constraintHeight_min="wrap"
    app:layout_constraintWidth_min="wrap"
 
    app:layout_constraintLeft_toLeftOf="parent"
    app:layout_constraintRight_toRightOf="parent"
    app:layout_constraintTop_toTopOf="parent"
    app:layout_constraintBottom_toBottomOf="parent"/>
```

Хотя в данном случае ширина TextView установлена в 260dp, поскольку максимальная ширина задана в 200dp, то реальная ширина не превысит 200dp.

### Размеры в процентах

Атрибут layout_constraintWidth_percent задает ширину элемента в процентах по отношению к доступному пространству по горизонтали. Аналогично атрибут layout_constraintHeight_percent задает высоту в процентах по отношению к доступному пространству по вертикали.

Для их применения необходимо соблюсти следующие условия:

-    Соответствующий атрибут для установки размера (android:layout_width - если мы устанавливаем ширину или android:layout_height - если мы устанавливаем ввысоту в процентах) должен иметь значение MATCH_CONSTRAINT или 0dp

-   Также необходимо установить атрибут app:layout_constraintWidth_default="percent" при установке ширины и app:layout_constraintHeight_default="percent" при установке высоты

В качестве значения атрибуты layout_constraintWidth_percent и layout_constraintHeight_percent принимают дробное число от 0 до 1.

Например, пусть TextView занимает по вертикали 25%, а по горизонтали 50% пространства:

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
        android:text="Hello Android"
        android:textSize="30sp"
        android:background="#e0e0e0"
         
        app:layout_constraintWidth_default="percent"
        app:layout_constraintHeight_default="percent"
         
        app:layout_constraintWidth_percent="0.5"
        app:layout_constraintHeight_percent="0.25"
         
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintBottom_toBottomOf="parent"/>
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Другой пример - пропорциональное разделение пространства между несколькими элементами:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <EditText
        android:id="@+id/editText"
        android:hint="Введите Email"
        android:layout_height="wrap_content"
         
        android:layout_width="0dp"
        app:layout_constraintWidth_default="percent"
        app:layout_constraintWidth_percent="0.66"
         
        app:layout_constraintRight_toLeftOf="@+id/button"
        app:layout_constraintTop_toTopOf="parent" />
    <Button
        android:id="@+id/button"
        android:text="Отправить"
        android:layout_height="wrap_content"
         
        android:layout_width="0dp"
        app:layout_constraintWidth_default="percent"
        app:layout_constraintWidth_percent="0.33"
         
        app:layout_constraintLeft_toRightOf="@id/editText"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

В данном случае текстового поле EditText будет занимать 66%, а кнопка - 33% ширины:

### Установка соотношения высоты и ширины

ConstraintLayout также позволяет устанавливать у элементов высоту относительно ширины / ширину относительно высоты. Для этого применяется атрибут layout_constraintDimensionRatio. В качестве значения он принимает отношение в виде Width:Height, например, 1:0.5 - здесь число 1 представляет ширину, а 0.5 - высоту. То есть ширина будет в два раза больше высоты. Но при этом хотя для одного измерения должно быть установлено 0dp (MATCH_CONSTRAINT). Например:

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
        android:layout_height="0dp"
        android:text="Hello Android"
        android:textSize="30sp"
        android:background="#e0e0e0"
        app:layout_constraintDimensionRatio="1:0.6"
 
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintBottom_toBottomOf="parent"/>
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

В данном случае ширина TextView будет такой, какая необходима для его содержимого, а высота 60% от ширины.

Если и для ширины, и для высоты установлено 0dp, то в этом случае система выберет наибольшее измерение, которое соответствует всем ограничениям, и относительно него установит значение другого измерения. Чтобы конкретизировать измерение, относительно которого будет идти расчет, можно указать символ W (ширина) или H (высота). Например:

```java
<TextView
    android:layout_width="0dp"
    android:layout_height="0dp"
    android:text="Hello Android"
    android:textSize="30sp"
    android:background="#e0e0e0"
         
    app:layout_constraintDimensionRatio="W, 1:4"
 
    app:layout_constraintLeft_toLeftOf="parent"
    app:layout_constraintRight_toRightOf="parent"
    app:layout_constraintTop_toTopOf="parent"
    app:layout_constraintBottom_toBottomOf="parent"/>
```

В данном случае ширина будет в 4 раза меньше высоты.

## 2.8 Java и Android | Цепочки элементов в ConstraintLayout

ConstraintLayout позволяет организовать расположение элементов в ряд по горизонтали или по вертикали или то, что в Android называется chains или цепочки. Мы можем по цепочке установить позиционирование одного элемента относительно другого и таким обазом организовать ряд элементов.

### Горизонтальная цепочка элементов

Например, ряд элементов по горизонтали:

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
        android:id="@+id/textView1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#efefef"
        android:text="First"
        android:textSize="30sp"
        app:layout_constraintRight_toLeftOf="@id/textView2"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
    <TextView
        android:id="@+id/textView2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#e0e0e0"
        android:text="Second"
        android:textSize="30sp"
        app:layout_constraintLeft_toRightOf="@id/textView1"
        app:layout_constraintRight_toLeftOf="@id/textView3"
        app:layout_constraintTop_toTopOf="parent" />
 
    <TextView
        android:id="@+id/textView3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#efefef"
        android:text="Third"
        android:textSize="30sp"
        app:layout_constraintLeft_toRightOf="@id/textView2"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

В итоге элементы цепочки равномерно будут растянуты по всей ширине контейнера:

Горизонтальная цепочка элементов достигается за счет двух факторов:

-    Первый элемент выравнивается относительно левой границы контейнера (app:layout_constraintLeft_toLeftOf="parent"), последний элемент выравнивается относительно правой границы контейнера (app:layout_constraintRight_toRightOf="parent").

-    Благодаря установке атрибутов app:layout_constraintLeft_toRightOf и app:layout_constraintRight_toLeftOf располагаем один элемент справа или слева от другого.

Кроме того, ConstraintLayout позволяет настроить положение элементов внутри цепочки. Для этого применяется атрибут layout_constraintHorizontal_chainStyle, который может принимать следующие значения:

-    spread: значение по умолчанию, при котором элементы цепочки равномерно растягиваются по всей длине цепочки, как в примере выше

-    spread_inside: первый и последний элемент цепочки примыкают к границами контейнера

-    packed: элементы цепочки располагаются вплотную друг к другу.

Например, применим значение spread_inside:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <TextView
        android:id="@+id/textView1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#efefef"
        android:text="First"
        android:textSize="30sp"
 
        app:layout_constraintHorizontal_chainStyle="spread_inside"
 
        app:layout_constraintRight_toLeftOf="@id/textView2"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
    <TextView
        android:id="@+id/textView2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#e0e0e0"
        android:text="Second"
        android:textSize="30sp"
        app:layout_constraintLeft_toRightOf="@id/textView1"
        app:layout_constraintRight_toLeftOf="@id/textView3"
        app:layout_constraintTop_toTopOf="parent" />
 
    <TextView
        android:id="@+id/textView3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#efefef"
        android:text="Third"
        android:textSize="30sp"
        app:layout_constraintLeft_toRightOf="@id/textView2"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Причем в данном случае достаточно установить атрибут у первого элемента цепочки:

Значение packed:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <TextView
        android:id="@+id/textView1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#efefef"
        android:text="First"
        android:textSize="30sp"
 
        app:layout_constraintHorizontal_chainStyle="packed"
 
        app:layout_constraintRight_toLeftOf="@id/textView2"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
    <TextView
        android:id="@+id/textView2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#e0e0e0"
        android:text="Second"
        android:textSize="30sp"
        app:layout_constraintLeft_toRightOf="@id/textView1"
        app:layout_constraintRight_toLeftOf="@id/textView3"
        app:layout_constraintTop_toTopOf="parent" />
 
    <TextView
        android:id="@+id/textView3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#efefef"
        android:text="Third"
        android:textSize="30sp"
        app:layout_constraintLeft_toRightOf="@id/textView2"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

### Вес элемента

Стоит отметить, что выше у элементов устанавливалась ширина, необходимая для их содержимого. Но мы могли бы установить и нулевую ширину, тогда элементы равномерно бы распределялись по всей цепочки без образования промежутков между ними.

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <TextView
        android:id="@+id/textView1"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:background="#efefef"
        android:text="First"
        android:textSize="30sp"
        app:layout_constraintRight_toLeftOf="@id/textView2"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
    <TextView
        android:id="@+id/textView2"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:background="#e0e0e0"
        android:text="Second"
        android:textSize="30sp"
        app:layout_constraintLeft_toRightOf="@id/textView1"
        app:layout_constraintRight_toLeftOf="@id/textView3"
        app:layout_constraintTop_toTopOf="parent" />
 
    <TextView
        android:id="@+id/textView3"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:background="#efefef"
        android:text="Third"
        android:textSize="30sp"
        app:layout_constraintLeft_toRightOf="@id/textView2"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

В этом случае значение атрибута app:layout_constraintHorizontal_chainStyle не играет никакой роли, так как все элементы итак растягиваются по всей цепочке.

Однако такое поведение может не устраивать, например, мы хотим, чтобы один элемент был два раза больше другого. И в этом случае мы можем с помощью атрибута layout_constraintHorizontal_weight. Однако следует учитывать, что при применении весов у элементов, они должны иметь нулевую ширину:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <TextView
        android:id="@+id/textView1"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:background="#efefef"
        android:text="First"
        android:textSize="30sp"
         
        app:layout_constraintHorizontal_weight="1"
         
        app:layout_constraintRight_toLeftOf="@id/textView2"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
    <TextView
        android:id="@+id/textView2"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:background="#e0e0e0"
        android:text="Second"
        android:textSize="30sp"
         
        app:layout_constraintHorizontal_weight="2"
         
        app:layout_constraintLeft_toRightOf="@id/textView1"
        app:layout_constraintRight_toLeftOf="@id/textView3"
        app:layout_constraintTop_toTopOf="parent" />
 
    <TextView
        android:id="@+id/textView3"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:background="#efefef"
        android:text="Third"
        android:textSize="30sp"
 
        app:layout_constraintHorizontal_weight="1"
         
        app:layout_constraintLeft_toRightOf="@id/textView2"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

В качестве значения атрибут layout_constraintHorizontal_weight принимает число - вес элемента. Так, в данном случае вес первого элемента - 1, вес второго - 2, а вес третьего - 1. Поэтому вся ширина контейнера будет условно поделена на 1 + 2 + 1 = 4 частей, из которых по одной части займут первый и третий элемент, а второй займет 2 части, то есть второй элемент будет в два раза больше первого и третьего элемента.

В принципе мы можем оставить элементы и с шириной "wrap_content" или конкретным значением, отличным от "0dp", просто в этом случае они не будут участвовать в распределении пространства контейнера и вес у такого элемента роли играть не будет.

### Вертикальная цепочка

Для образования вертикальной цепочки также должно соблюдаться два условия:

-    Первый элемент выравнивается относительно верхней границы контейнера (app:layout_constraintTop_toTopOf="parent"), последний элемент выравнивается относительно нижней границы контейнера (app:layout_constraintBottom_toBottomOf="parent").

-    Благодаря установке атрибутов app:layout_constraintBottom_toTopOf и app:layout_constraintBottom_toTopOf располагаем один элемент поверх другого.

Чтобы настроить положение элементов внутри цепочки, применяется атрибут layout_constraintVertical_chainStyle, который может принимать следующие значения:

-    spread: значение по умолчанию, при котором элементы цепочки равномерно растягиваются по всей длине цепочки

-    spread_inside: первый и последний элемент цепочки примыкают к границами контейнера

 -   packed: элементы цепочки прилегают вплотную друг к другу.

Например, вертикальная цепочка со значением по умолчанию - spread:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <TextView
        android:id="@+id/textView1"
        android:layout_width="200dp"
        android:layout_height="wrap_content"
        android:background="#efefef"
        android:text="First"
        android:textSize="30sp"
        app:layout_constraintBottom_toTopOf="@id/textView2"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
    <TextView
        android:id="@+id/textView2"
        android:layout_width="200dp"
        android:layout_height="wrap_content"
        android:background="#e0e0e0"
        android:text="Second"
        android:textSize="30sp"
        app:layout_constraintTop_toBottomOf="@id/textView1"
        app:layout_constraintBottom_toTopOf="@id/textView3"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent" />
 
    <TextView
        android:id="@+id/textView3"
        android:layout_width="200dp"
        android:layout_height="wrap_content"
        android:background="#efefef"
        android:text="Third"
        android:textSize="30sp"
 
        app:layout_constraintTop_toBottomOf="@id/textView2"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintBottom_toBottomOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Также достаточно применить к первому элементу цепочки атрибут layout_constraintVertical_chainStyle, чтобы изменить положение элементов:

```java
<TextView
        android:id="@+id/textView1"
        android:layout_width="200dp"
        android:layout_height="wrap_content"
        android:background="#efefef"
        android:text="First"
        android:textSize="30sp"
         
        app:layout_constraintVertical_chainStyle="spread_inside"
         
        app:layout_constraintBottom_toTopOf="@id/textView2"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
```

И как при горизонтальной ориентации в вертикальной цепочки можно использовать вес элементов с помощью атрибута layout_constraintVertical_weight. Для установки веса у элемента в качестве высоты должно быть установлено значение 0dp

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
 
    <TextView
        android:id="@+id/textView1"
        android:layout_width="200dp"
        android:layout_height="0dp"
        android:background="#efefef"
        android:text="First"
        android:textSize="30sp"
        app:layout_constraintVertical_weight="1"
        app:layout_constraintBottom_toTopOf="@id/textView2"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
    <TextView
        android:id="@+id/textView2"
        android:layout_width="200dp"
        android:layout_height="0dp"
        android:background="#e0e0e0"
        android:text="Second"
        android:textSize="30sp"
        app:layout_constraintVertical_weight="3"
        app:layout_constraintTop_toBottomOf="@id/textView1"
        app:layout_constraintBottom_toTopOf="@id/textView3"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent" />
 
    <TextView
        android:id="@+id/textView3"
        android:layout_width="200dp"
        android:layout_height="0dp"
        android:background="#efefef"
        android:text="Third"
        android:textSize="30sp"
        app:layout_constraintVertical_weight="2"
        app:layout_constraintTop_toBottomOf="@id/textView2"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintBottom_toBottomOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Совокупный вес элементов в данном случае 1 + 3 + 2 = 6. Поэтому вся высота контейнера будет делиться на 6 частей, из которых первый элемент займет 1 часть, второй - 3 части и третий - 2 части в соответствии со своим весом.

## 2.9 Java и Android | Программное создание ConstraintLayout и позиционионирование

Для создания контейнера в коде Java применяется одноименный класс ConstraintLayout, для создания объекта которого в конструктор передаются значения для ширины и высоты элемента:

```java
ConstraintLayout.LayoutParams layoutParams = new ConstraintLayout.LayoutParams
                (ConstraintLayout.LayoutParams.WRAP_CONTENT , ConstraintLayout.LayoutParams.WRAP_CONTENT);
```

Первый параметр устанавливает щирину элемента, а второй - высоту. ConstraintLayout.LayoutParams.WRAP_CONTENT указывает, что элемент будет иметь те размеры, которые необходимы для того, чтобы вывести на экран его содержимое. Кроме ConstraintLayout.LayoutParams.WRAP_CONTENT можно применять константу ConstraintLayout.LayoutParams.MATCH_CONSTRAINT, которая аналогична применению значения "0dp" в атрибутах layout_width и layout_height и которая растягивает элемент по ширине или высоте контейнера.

Также можно использовать точные размеры, например:

```java
ConstraintLayout.LayoutParams layoutParams = new ConstraintLayout.LayoutParams
                (ConstraintLayout.LayoutParams.MATCH_CONSTRAINT, 200);
```

Для настройки позиционирования внутри ConstraintLayout применяется класс ConstraintLayout.LayoutParams. Он имеет довольно много функционала. Рассмотрим в данном случае только те поля, которые позволяют установить расположение элемента:

-    baselineToBaseline: выравнивает базовую линию элемента по базовой линии другого элемента, id которого присваивается свойству.

-    bottomToBottom: выравнивает нижнюю границу элемента по нижней границе другого элемента.

-    bottomToTop: выравнивает нижнюю границу элемента по верхней границе другого элемента.

-    leftToLeft: выравнивает левую границу элемента по левой границе другого элемента.

-    leftToRight: выравнивает левую границу элемента по правой границе другого элемента.

-    rightToLeft: выравнивает правую границу элемента по левой границе другого элемента.

-    rightToRight: выравнивает правую границу элемента по правой границе другого элемента.

-    startToEnd: выравнивает начало элемента по завершению другого элемента.

-    startToStart: выравнивает начало элемента по началу другого элемента.

-    topToBottom: выравнивает верхнюю границу элемента по нижней границе другого элемента.

-    topToTop: выравнивает верхнюю границу элемента по верхней границе другого элемента.

-    endToEnd: выравнивает заврешение элемента по завершению другого элемента.

-    endToStart: выравнивает завершение элемента по началу другого элемента.

В качестве значения эти поля принимают id (идентификатор) элемента, относительно которого выполняется позиционирование. Если расположение устанавливается относительно контейнера ConstraintLayout, то применяется константа ConstraintLayout.LayoutParams.PARENT_ID

Рассмотрим простейший пример:

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
        //setContentView(R.layout.activity_main);
 
        ConstraintLayout constraintLayout = new ConstraintLayout(this);
        TextView textView = new TextView(this);
        // установка текста текстового поля
        textView.setText("Hello Android");
        // установка размера текста
        textView.setTextSize(30);
 
        ConstraintLayout.LayoutParams layoutParams = new ConstraintLayout.LayoutParams
                (ConstraintLayout.LayoutParams.WRAP_CONTENT , ConstraintLayout.LayoutParams.WRAP_CONTENT);
        // позиционирование в левом верхнем углу контейнера
        // эквивалент app:layout_constraintLeft_toLeftOf="parent"
        layoutParams.leftToLeft = ConstraintLayout.LayoutParams.PARENT_ID;
        // эквивалент app:layout_constraintTop_toTopOf="parent"
        layoutParams.topToTop = ConstraintLayout.LayoutParams.PARENT_ID;
        // устанавливаем размеры
        textView.setLayoutParams(layoutParams);
        // добавляем TextView в ConstraintLayout
        constraintLayout.addView(textView);
 
        setContentView(constraintLayout);
    }
}
```

В данном случае значение ConstraintLayout.LayoutParams.WRAP_CONTENT для ширины и высоты указывает, что элемент будет иметь те размеры, которые необходимы для того, чтобы вывести на экран его содержимое.

Далее выравниваем левую границу элемента по левой стороне контейнера:

```java
layoutParams.leftToLeft = ConstraintLayout.LayoutParams.PARENT_ID;
```

Эта установка аналогична использованию атрибута app:layout_constraintLeft_toLeftOf="parent".

Затем выравниваем верхнюю границу элемента по верхней стороне контейнера:

```java
layoutParams.topToTop = ConstraintLayout.LayoutParams.PARENT_ID;
```

Эта установка аналогична использованию атрибута app:layout_constraintTop_toTopOf="parent".

И в конце применяем объект ConstraintLayout.LayoutParams к TextView:

```java
constraintLayout.addView(textView);
```

В итоге элемент TextView будет расположен в верхнем левом углу ConstraintLayout:

Рассмотрим другой пример - установку расположения элементов относительно друг друга:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import androidx.constraintlayout.widget.ConstraintLayout;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        //setContentView(R.layout.activity_main);
 
        ConstraintLayout constraintLayout = new ConstraintLayout(this);
 
        EditText editText = new EditText(this);
        editText.setHint("Введите Email");
        editText.setId(View.generateViewId());
         
        Button button = new Button(this);
        button.setText("Отправить");
        button.setId(View.generateViewId());
 
        ConstraintLayout.LayoutParams editTextLayout = new ConstraintLayout.LayoutParams
                (ConstraintLayout.LayoutParams.WRAP_CONTENT , ConstraintLayout.LayoutParams.WRAP_CONTENT);
        editTextLayout.leftToLeft = ConstraintLayout.LayoutParams.PARENT_ID;
        editTextLayout.topToTop = ConstraintLayout.LayoutParams.PARENT_ID;
        editTextLayout.rightToLeft = button.getId();
        editText.setLayoutParams(editTextLayout);
        constraintLayout.addView(editText);
 
        ConstraintLayout.LayoutParams buttonLayout = new ConstraintLayout.LayoutParams
                (ConstraintLayout.LayoutParams.WRAP_CONTENT , ConstraintLayout.LayoutParams.WRAP_CONTENT);
        buttonLayout.leftToRight = editText.getId();
        buttonLayout.topToTop = ConstraintLayout.LayoutParams.PARENT_ID;
        button.setLayoutParams(buttonLayout);
        constraintLayout.addView(button);
 
        setContentView(constraintLayout);
    }
}
```

При расположении одного элемента относительно другого, нам нужно знать id вторрого элемента. Если элемент определен в коде Java, то вначале надо сгенерировать идентификатор:

```java
editText.setId(View.generateViewId());
button.setId(View.generateViewId());
```

Затем можно применять идентификаторы элементов для установки позиционирование позиционионирование. Так, правая граница EditText выравнивается по левой границе кнопки:

```java
editTextLayout.rightToLeft = button.getId();
```

А левая граница кнопки выравнивается по правой границе элемента EditText:

```java
buttonLayout.leftToRight = editText.getId();
```

## 2.10 Java и Android | LinearLayout

Контейнер LinearLayout представляет простейший контейнер - объект ViewGroup, который упорядочивает все дочерние элементы в одном направлении: по горизонтали или по вертикали. Все элемены расположены один за другим. Направление разметки указывается с помощью атрибута android:orientation.

Если, например, ориентация разметки вертикальная (android:orientation="vertical"), то все элементы располагаются в столбик - по одному элементу на каждой строке. Если ориентация горизонтальная (android:orientation="horizontal"), то элементы располагаются в одну строку. Например, расположим элементы в горизонтальный ряд:

```java
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="horizontal" >
 
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_margin="5dp"
        android:text="Hello"
        android:textSize="26sp" />
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_margin="5dp"
        android:text="Android"
        android:textSize="26sp" />
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_margin="5dp"
        android:text="World"
        android:textSize="26sp" />
</LinearLayout>
```

Если бы мы указали для LinearLayout атрибут android:orientation="vertical", то элементы размещались бы по вертикали:

### Вес элемента

LinearLayout поддерживает такое свойство, как вес элемента, которое передается атрибутом android:layout_weight. Это свойство принимает значение, указывающее, какую часть оставшегося свободного места контейнера по отношению к другим объектам займет данный элемент. Например, если один элемент у нас будет иметь для свойства android:layout_weight значение 2, а другой - значение 1, то в сумме они дадут 3, поэтому первый элемент будет занимать 2/3 оставшегося пространства, а второй - 1/3.

Если все элементы имеют значение android:layout_weight="1", то все эти элементы будут равномерно распределены по всей площади контейнера:

```java
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical" >
    <TextView
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:text="Hello"
        android:background="#e0e0e0"
        android:layout_weight="1"
        android:textSize="26sp" />
    <TextView
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:background="#eeeeee"
        android:text="Android"
        android:layout_weight="1"
        android:textSize="26sp" />
    <TextView
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:text="World"
        android:background="#bdbdbd"
        android:layout_weight="1"
        android:textSize="26sp" />
</LinearLayout>
```

В данном случае LinearLayout имеет вертикальную ориентацию, поэтому все элементы будут располагаться сверху вниз. Все три элемента имеют значение android:layout_weight="1", поэтому сумма весов всех элементов будет равна 3, а каждый элемент получит по трети пространства в LinearLayout:

При этом так как у нас вертикальный стек, то нам надо также установить для свойства layout_height значение 0dp. Если бы LinearLayout имел горизонтальную ориентацию, то для свойства layout_width надо было бы установить значение 0dp.

Еще один атрибут android:weightSum позволяет указать сумму весов всех элементов. Например:

```java
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:weightSum="7">
 
    <TextView
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:text="Hello"
        android:background="#e0e0e0"
        android:layout_weight="1"
        android:textSize="26sp" />
    <TextView
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:background="#eeeeee"
        android:text="Android"
        android:layout_weight="3"
        android:textSize="26sp" />
    <TextView
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:text="World"
        android:background="#bdbdbd"
        android:layout_weight="2"
        android:textSize="26sp" />
</LinearLayout>
```

LinearLayout здесь задает сумму весов равную 7. То есть все пространство по вертикали (так как вертикальная ориентация) условно делится на семь равных частей.

Первый TextView имеет вес 1, то есть из этих семи частей занимает только одну. Второй TextView имеет вес 3, то есть занимает три части из семи. И третий имеет вес 2. Итоговая сумма составляет 6. Но так как LinearLayout задает вес 7, то одна часть будет свободна от всех элементов.

### Программное создание LinearLayout

Создание LinearLayout в коде java:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.LinearLayout;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        //setContentView(R.layout.activity_main);
        LinearLayout linearLayout = new LinearLayout(this);
        // горизонтальная ориентация
        linearLayout.setOrientation(LinearLayout.HORIZONTAL);
         
        TextView textView = new TextView(this);
        textView.setText("Hello");
        textView.setTextSize(30);
        // создаем параметры позиционирования для элемента
        LinearLayout.LayoutParams layoutParams = new LinearLayout.LayoutParams
                (LinearLayout.LayoutParams.WRAP_CONTENT, LinearLayout.LayoutParams.WRAP_CONTENT);
        // устанавливаем отступы
        layoutParams.setMargins(100, 100, 0, 0);
        textView.setLayoutParams(layoutParams);
        // добавляем элемент в LinearLayout
        linearLayout.addView(textView);
 
        setContentView(linearLayout);
    }
}
```

Дополнительная версия конструктора LinearLayout.LayoutParams() в качестве третьего параметра позволяет указать вес элемента:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.LinearLayout;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
         
        LinearLayout linearLayout = new LinearLayout(this);
        linearLayout.setOrientation(LinearLayout.VERTICAL);
         
        // первое текстовое поле
        TextView textView1 = new TextView(this);
        textView1.setText("Hello");
        textView1.setTextSize(30);
        // textView1 имеет вес 3
        linearLayout.addView(textView1, new LinearLayout.LayoutParams
                (LinearLayout.LayoutParams.MATCH_PARENT, 0, 3));
 
        // второе текстовое поле
        TextView textView2 = new TextView(this);
        textView2.setText("Android");
        textView2.setBackgroundColor(0xFFBDBDBD);
        textView2.setTextSize(30);
        // textView2 имеет вес 2
        linearLayout.addView(textView2, new LinearLayout.LayoutParams
                (LinearLayout.LayoutParams.MATCH_PARENT, 0, 2));
 
        setContentView(linearLayout);
    }
}
```

### Layout_gravity

Атрибут layout_gravity позволяет устанавливать позиционирование относительно LinearLayout. Он принимает следуюшие значения:

-    top: выравнивает элемент по верхней границе контейнера

-    bottom: выравнивает элемент по нижней границе контейнера

-    left: выравнивает элемент по левой границе контейнера

-    right: выравнивает элемент по правой границе контейнера

-   center_vertical: выравнивает элемент по центру по вертикали

-    center_horizontal: выравнивает элемент по центру по горизонтали

-    center: элемент позиционируется в центре

-    fill_vertical: элемент растягивается по вертикали

-    fill_horizontal: элемент растягивается по горизонтали

-    fill: элемент заполняет все пространство контейнера

-    clip_vertical: обрезает верхнюю и нижнюю границу элемента

-    clip_horizontal: обрезает правую и левую границу элемента

-    start: элемент позиционируется в начале (в верхнем левом углу) контейнера

-    end: элемент позиционируется в конце контейнера (в верхнем правом углу)

Например:

```java
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical">
    <TextView
        android:layout_gravity="left"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="30sp"
        android:text="Hello Java!"
        android:background="#e8eaf6"/>
    <TextView
        android:layout_gravity="center"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="30sp"
        android:text="Hello World!"
        android:background="#e8eaf6"/>
    <TextView
        android:layout_gravity="right"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="30sp"
        android:text="Hello Android!"
        android:background="#e8eaf6"/>
    <TextView
        android:layout_gravity="center"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="30sp"
        android:text="Hello Kotlin!"
        android:background="#e8eaf6"/>
</LinearLayout>
```

В данном случае первый элемент TextView будет позиционироваться по левой стороне контейнера (android:layout_gravity="left"), второй TextView по центру (android:layout_gravity="center"), третий - по правой стороне (android:layout_gravity="right") и четвертый - по центру (android:layout_gravity="center")

Стоит учитывать ориентацию контейнера. Например, при вертикальной ориентации все элементы будут представлять вертикальный стек, идущий сверху вниз. Поэтому значения, которые относятся к позиционированию элемента по вертикали (например, top или bottom) никак не будут влиять на элемент. Также при горизонтальной ориентации LinearLayout не окажут никакого влияния значения, которые позиционируют элемент по горизонтали, например, left и right.

Для установки программно параметра layout_gravity надо задать поле gravity у объекта LinearLayout.LayoutParams:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.Gravity;
import android.widget.LinearLayout;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
 
        LinearLayout linearLayout = new LinearLayout(this);
        linearLayout.setOrientation(LinearLayout.VERTICAL);
        LinearLayout.LayoutParams layoutParams = new LinearLayout.LayoutParams
                (LinearLayout.LayoutParams.WRAP_CONTENT, LinearLayout.LayoutParams.WRAP_CONTENT);
// установка layout_gravity
        layoutParams.gravity = Gravity.CENTER;
        // первое текстовое поле
        TextView textView1 = new TextView(this);
        textView1.setText("Hello");
        textView1.setTextSize(30);
        linearLayout.addView(textView1, layoutParams);
        setContentView(linearLayout);
    }
}
```

В качестве значения передается одна из констант класса Gravity, которые аналогичны значениям атрибута.

## 2.11 Java и Android | RelativeLayout

RelativeLayout представляет объект ViewGroup, который располагает дочерние элементы относительно позиции других дочерних элементов разметки или относительно области самой разметки RelativeLayout. Используя относительное позиционирование, мы можем установить элемент по правому краю или в центре или иным способом, который предоставляет данный контейнер. Для установки элемента в файле xml мы можем применять следующие атрибуты:

-    android:layout_above: располагает элемент над элементом с указанным Id

-    android:layout_below: располагает элемент под элементом с указанным Id

-    android:layout_toLeftOf: располагается слева от элемента с указанным Id

-    android:layout_toRightOf: располагается справа от элемента с указанным Id

-    android:layout_toStartOf: располагает начало текущего элемента, где начинается элемент с указанным Id

-    android:layout_toEndOf: располагает начало текущего элемента, где завершается элемент с указанным Id

-    android:layout_alignBottom: выравнивает элемент по нижней границе другого элемента с указанным Id

-    android:layout_alignLeft: выравнивает элемент по левой границе другого элемента с указанным Id

-    android:layout_alignRight: выравнивает элемент по правой границе другого элемента с указанным Id

-    android:layout_alignStart: выравнивает элемент по линии, у которой начинается другой элемент с указанным Id

-    android:layout_alignEnd: выравнивает элемент по линии, у которой завершается другой элемент с указанным Id

-   android:layout_alignTop: выравнивает элемент по верхней границе другого элемента с указанным Id

-    android:layout_alignBaseline: выравнивает базовую линию элемента по базовой линии другого элемента с указанным Id

-    android:layout_alignParentBottom: если атрибут имеет значение true, то элемент прижимается к нижней границе контейнера

-   android:layout_alignParentRight: если атрибут имеет значение true, то элемент прижимается к правому краю контейнера

-   android:layout_alignParentLeft: если атрибут имеет значение true, то элемент прижимается к левому краю контейнера

-   android:layout_alignParentStart: если атрибут имеет значение true, то элемент прижимается к начальному краю контейнера (при левосторонней ориентации текста - левый край)

-    android:layout_alignParentEnd: если атрибут имеет значение true, то элемент прижимается к конечному краю контейнера (при левосторонней ориентации текста - правый край)

-    android:layout_alignParentTop: если атрибут имеет значение true, то элемент прижимается к верхней границе контейнера

-    android:layout_centerInParent: если атрибут имеет значение true, то элемент располагается по центру родительского контейнера

-    android:layout_centerHorizontal: при значении true выравнивает элемент по центру по горизонтали

-    android:layout_centerVertical: при значении true выравнивает элемент по центру по вертикали

Например, позиционирование относительно контейнера RelativeLayout:

```java
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
 
    <TextView android:text="Left Top"
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:textSize="26sp"
        android:layout_alignParentLeft="true"
        android:layout_alignParentTop="true" />
 
    <TextView android:text="Right Top"
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:textSize="26sp"
        android:layout_alignParentRight="true"
        android:layout_alignParentTop="true" />
 
    <TextView android:text="Left Bottom"
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:textSize="26sp"
        android:layout_alignParentLeft="true"
        android:layout_alignParentBottom="true" />
 
    <TextView android:text="Right Bottom"
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:textSize="26sp"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true" />
</RelativeLayout>
```

Для позиционирования относительно другого элемента, нам надо указать id этого элемента. Так, поместим на RelativeLayout текстовое поле и кнопку:

```java
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
 
    <EditText
        android:id="@+id/edit_message"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_centerInParent="true"/>
    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Отправить"
        android:layout_alignRight="@id/edit_message"
        android:layout_below="@id/edit_message"
        />
</RelativeLayout>
```

В данном случае поле EditText располагается по центру в RelativeLayout, а кнопка помещается под EditText и выравнивается по его правой границе:

### Программное создание RelativeLayout

Создадим элемент RelativeLayout программно в коде Java:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.Button;
import android.widget.EditText;
import android.widget.RelativeLayout;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
         
        RelativeLayout relativeLayout = new RelativeLayout(this);
 
        EditText editText = new EditText(this);
        editText.setId(EditText.generateViewId());
 
        Button button = new Button(this);
        button.setText("Отправить");
 
        // устанавливаем параметры положения для EditText
        RelativeLayout.LayoutParams editTextParams = new RelativeLayout.LayoutParams(
                RelativeLayout.LayoutParams.MATCH_PARENT,
                RelativeLayout.LayoutParams.WRAP_CONTENT
        );
        // выравнивание по центру родительского контейнера
        editTextParams.addRule(RelativeLayout.CENTER_IN_PARENT);
        // добавляем в RelativeLayout
        relativeLayout.addView(editText, editTextParams);
 
        // устанавливаем параметры положения для Button
        RelativeLayout.LayoutParams buttonParams = new RelativeLayout.LayoutParams(
                RelativeLayout.LayoutParams.WRAP_CONTENT,
                RelativeLayout.LayoutParams.WRAP_CONTENT
        );
        // выравнивание справа и снизу от поля EditText
        buttonParams.addRule(RelativeLayout.BELOW, editText.getId());
        buttonParams.addRule(RelativeLayout.ALIGN_RIGHT, editText.getId());
        // добавляем в RelativeLayout
        relativeLayout.addView(button, buttonParams);
 
        setContentView(relativeLayout);
    }
}
```

Чтобы задать положение элемента в контейнере, применяется класс RelativeLayout.LayoutParams. Через конструктор устанавливаются значения для для ширины и высоты. Например, у элемента EditText для ширины устанавливается значение MATCH_PARENT, а для высоты - WRAP_CONTENT.

С помощью метода addRule() мы можем добавлять дополнительные правила для позиционирования элемента. Этот метод в качестве параметра принимает числовую константу, которая представляет параметр позиционирования и которая аналогична атрибуту. Например, атрибуту android:layout_centerInParent будет соответствовать константа CENTER_IN_PARENT, а атрибуту android:layout_alignRight константа ALIGN_RIGHT.

Стоит отметить, что в целях упрощения кода для установки id у EditText вызывается метод generateViewId();, который позволяет программно сгенерировать id для элемента управления.

Затем установленный id передается в качестве второго параметра в метод addRule при установке правил для кнопки:

```java
buttonParams.addRule(RelativeLayout.BELOW, editText.getId());
```

Тем самым мы указываем относительно какого элемента надо задать расположение.

## 2.12 Java и Android | TableLayout

Контейнер TableLayout структурирует элементы управления в виде таблицы по столбцам и строкам. Определим в файле activity_main.xml элемент TableLayout, который будет включать две строки и два столбца:

```java
<TableLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent" 
    android:layout_height="match_parent">
    <TableRow>
        <TextView
            android:layout_weight="0.5"
            android:text="Логин"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content" />
 
        <EditText
            android:layout_weight="1"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"  />
    </TableRow>
 
    <TableRow>
        <TextView
            android:layout_weight="0.5"
            android:text="Email"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content" />
 
        <EditText
            android:layout_weight="1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content" />
    </TableRow>
</TableLayout>
```

Используя элемент TableRow, мы создаем отдельную строку. Как разметка узнает сколько столбцов надо создать? Android находит строку с максимальным количеством виджетов одного уровня, и это количество будет означать количество столбцов. Например, в данном случае у нас определены две строки и в каждой по два элемента. Если бы в какой-нибудь из них было бы три виджета, то соответственно столбцов было бы также три, даже если в другой строке осталось бы два виджета.

Причем элемент TableRow наследуется от класса LinearLayout, поэтому мы можем к нему применять тот же функционал, что и к LinearLayout. В частности, для определения пространства для элементов в строке используется атрибут android:layout_weight.

Если какой-то элемент должен быть растянут на ряд столбцов, то мы можем растянуть его с помощью атрибута layout_span, который указывает на какое количество столбцов надо растянуть элемент:

```java
<TableLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
    <TableRow>
        <TextView
            android:textSize="22sp"
            android:text="Логин"
            android:layout_width="100dp"
            android:layout_height="wrap_content" />
 
        <EditText
            android:textSize="22sp"
            android:layout_width="200dp"
            android:layout_height="wrap_content"  />
    </TableRow>
 
    <TableRow>
        <TextView
            android:textSize="22sp"
            android:text="Email"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content" />
 
        <EditText
            android:textSize="22sp"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content" />
    </TableRow>
    <TableRow>
        <Button
            android:text="Отправить"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_span="2"/>
    </TableRow>
</TableLayout> 
```

Также можно растянуть элемент на всю строку, установив у него атрибут android:layout_weight="1":

```java
<TableRow>
    <Button
        android:text="Отправить"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_weight="1" />
</TableRow>
```

### Программное создание TableLayout

Создадим TableLayout программным образом, переложив на код java самый первый пример из данной статьи:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.EditText;
import android.widget.TableLayout;
import android.widget.TableRow;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
 
        TableLayout tableLayout = new TableLayout( this);
         
        // первая строка
        TableRow tableRow1 = new TableRow(this);
 
        TextView textView1 = new TextView(this);
        textView1.setText("Логин");
        tableRow1.addView(textView1, new TableRow.LayoutParams(
                TableRow.LayoutParams.WRAP_CONTENT, TableRow.LayoutParams.WRAP_CONTENT, 0.5f));
 
        EditText editText1 = new EditText(this);
        tableRow1.addView(editText1, new TableRow.LayoutParams(
                TableRow.LayoutParams.WRAP_CONTENT, TableRow.LayoutParams.WRAP_CONTENT, 1.0f));
 
        // вторая строка
        TableRow tableRow2 = new TableRow(this);
 
        TextView textView2 = new TextView(this);
        textView2.setText("Email");
        tableRow2.addView(textView2, new TableRow.LayoutParams(
                TableRow.LayoutParams.WRAP_CONTENT, TableRow.LayoutParams.WRAP_CONTENT, 0.5f));
 
        EditText editText2 = new EditText(this);
        tableRow2.addView(editText2, new TableRow.LayoutParams(
                TableRow.LayoutParams.WRAP_CONTENT, TableRow.LayoutParams.WRAP_CONTENT, 1.f));
 
        tableLayout.addView(tableRow1);
        tableLayout.addView(tableRow2);
        setContentView(tableLayout);
    }
}
```

## 2.13 Java и Android | FrameLayout

Контейнер FrameLayout предназначен для вывода на экран одного помещенного в него визуального элемента. Если же мы поместим несколько элементов, то они будут накладываться друг на друга. Тем не менее также можно располагать в FrameLayout несколько элементов.

Допустим, вложим в FrameLayout два элемента TextView:

```java
<?xml version="1.0" encoding="utf-8"?>
<FrameLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
 
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        android:textSize="26sp"/>
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello Android!"
        android:textSize="26sp"
        android:layout_marginTop="50dp"/>
 
</FrameLayout>
```

Здесь оба элемента позиционируются в одно и то же место - в левый верхний угол контейнера FrameLayout, и чтобы избежать наложения, в данном случае у второго TextView устанавливается отступ сверху в 50 единиц.

Нередко FrameLayout применяется для создания производных контейнеров, например, ScrollView, который обеспечивает прокрутку.

Элементы управления, которые помещаются в FrameLayout, могут установить свое позиционирование с помощью атрибута android:layout_gravity:

```java
<?xml version="1.0" encoding="utf-8"?>
<FrameLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
 
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        android:textSize="26sp"
        android:layout_gravity="center_horizontal" />
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Welcome to Java World"
        android:textSize="26sp"
        android:layout_gravity="center"/>
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello Android!"
        android:textSize="26sp"
        android:layout_gravity="bottom|center_horizontal"/>
 
</FrameLayout>
```

При указании значения мы можем комбинировать ряд значений, разделяя их вертикальной чертой: bottom|center_horizontal

Программное создание FrameLayout в коде MainActivity:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.view.Gravity;
import android.widget.FrameLayout;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
 
        FrameLayout frameLayout = new FrameLayout(this);
        TextView textView = new TextView(this);
        textView.setText("Hello World!");
 
        FrameLayout.LayoutParams layoutParams = new FrameLayout.LayoutParams
                (FrameLayout.LayoutParams.WRAP_CONTENT, FrameLayout.LayoutParams.WRAP_CONTENT);
        layoutParams.gravity = Gravity.CENTER_HORIZONTAL | Gravity.TOP;
 
        textView.setLayoutParams(layoutParams);
        textView.setTextSize(26);
        frameLayout.addView(textView);
        setContentView(frameLayout);
    }
}
```

## 2.14 Java и Android | GridLayout

GridLayout представляет еще один контейнер, который позволяет создавать табличные представления. GridLayout состоит из коллекции строк, каждая из которых состоит из отдельных ячеек:

```java
<GridLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:rowCount="3"
    android:columnCount="3">
 
    <Button android:text="1" />
    <Button android:text="2" />
    <Button android:text="3" />
    <Button android:text="4" />
    <Button android:text="5" />
    <Button android:text="6" />
    <Button android:text="7" />
 
    <Button android:text="8" />
 
    <Button android:text="9" />
</GridLayout>
```

С помощью атрибутов android:rowCount и android:columnCount устанавливается число строк и столбцов соответственно. Так, в данном случае устанавливаем 3 строки и 3 столбца. GridLayout автоматически может позиционировать вложенные элементы управления по строкам. Так, в нашем случае первая кнопка попадает в первую ячейку (первая строка первый столбец), вторая кнопка - во вторую ячейку и так далее.

При этом ширина столбцов устанавливается автоматически по ширине самого широкого элемента.

Однако мы можем явно задать номер столбца и строки для определенного элемента, а при необходимости растянуть на несколько столбцов или строк. Для этого мы можем применять следующие атрибуты:

- android:layout_column: номер столбца (отсчет идет от нуля)

- android:layout_row: номер строки

- android:layout_columnSpan: количество столбцов, на которые растягивается элемент

- android:layout_rowSpan: количество строк, на которые растягивается элемент

Например:

```java
<GridLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:rowCount="3"
    android:columnCount="3">
 
    <Button
        android:text="1"
        android:layout_column="0"
        android:layout_row="0" />
    <Button android:text="2"
        android:layout_column="1"
        android:layout_row="0"/>
    <Button android:text="3"
        android:layout_column="2"
        android:layout_row="0"  />
    <Button android:text="4"
        android:layout_width="180dp"
        android:layout_columnSpan="2"/>
    <Button android:text="5"
        android:layout_height="100dp"
        android:layout_rowSpan="2"/>
    <Button android:text="6" />
    <Button android:text="7"/>
</GridLayout>
```

### Программное создание GridLayout

Среди методов GridLayout следует отметить методы setRowCount() и setColumnCount(), которые позволяют задать соответственно количество строк и столбцов. Например, определим в коде GridLayout, аналогичнй первому примеру в статье:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.Gravity;
import android.widget.Button;
import android.widget.EditText;
import android.widget.GridLayout;
import android.widget.LinearLayout;
import android.widget.TableLayout;
import android.widget.TableRow;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
 
        GridLayout gridLayout = new GridLayout( this);
        // количество строк
        gridLayout.setRowCount(3);
        // количество столбцов
        gridLayout.setColumnCount(3);
 
        for(int i = 1; i <=9; i++){
            Button btn = new Button(this);
            btn.setText(String.valueOf(i));
            gridLayout.addView(btn);
        }
        setContentView(gridLayout);
    }
}
```

В данном случае GridLayout имеет три строки и три столбца. При добавлении виджетов (в данном случае кнопок) они последовательно помещаются в ячейки грида по одному виджету в ячейке.

### GridLayout.LayoutParams

Для более детальной настройки расположения виджета в гриде можно использовать класс GridLayout.LayoutParams. Этот класс имеет ряд свойств, которые позволяют настроить расположение:

- columnSpec: задает столбец для расположения в виде объекта GridLayout.Spec

- rowSpec: задает строку для расположения в виде объекта GridLayout.Spec

- leftMargin: задает отступ слева

- rightMargin: задает отступ справа

- topMargin: задает отступ сверху

- bottomMargin: задает отступ снизу

- width: задает ширину виджета

- height: задает высоту виджета

Объект GridLayout.Spec позволяет задать размещение в ячейках столбца или строки. Для создание этого объекта применяется статический метод GridLayout.spec(), который имеет ряд версий. Отметим среди них следующие:

- GridLayout.spec(int): задает столбец или строку, где располагается виджет. Отсчет ячеек начинается с нуля. Виджет занимает только одну ячейку

- GridLayout.spec(int, int): первый параметр задает столбец или строку, где располагается виджет. Второй параметр указывает, насколько ячеек растягивается виджет

- GridLayout.spec(int, android.widget.GridLayout.Alignment): первый параметр задает столбец или строку, где располагается виджет. Второй параметр устанавливает выравнивание виджета

- GridLayout.spec(int, int, android.widget.GridLayout.Alignment): первый параметр задает столбец или строку, где располагается виджет. Второй параметр указывает, насколько ячеек растягивается виджет. Третий параметр устанавливает выравнивание виджета

Пример применения GridLayout.LayoutParams:

```java
Button btn = new Button(this);
btn.setText("нажми");
GridLayout.LayoutParams layoutParams = new GridLayout.LayoutParams();
 // кнопка помещается в нулевой столбец и растягивается на 2 столбца
layoutParams.columnSpec = GridLayout.spec(0,2);
 // кнопка помещается во вторую строку и растягивается на 1 строку
layoutParams.rowSpec = GridLayout.spec(1,1);
layoutParams.leftMargin=5;
layoutParams.rightMargin=5;
layoutParams.topMargin=4;
layoutParams.bottomMargin=4;
layoutParams.width = GridLayout.LayoutParams.MATCH_PARENT;
layoutParams.height = GridLayout.LayoutParams.WRAP_CONTENT;
gridLayout.addView(btn, layoutParams);
```

Например, реализуем в коде второй пример из данной статьи:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.util.TypedValue;
import android.view.Gravity;
import android.widget.Button;
import android.widget.EditText;
import android.widget.GridLayout;
import android.widget.LinearLayout;
import android.widget.TableLayout;
import android.widget.TableRow;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
 
        GridLayout gridLayout = new GridLayout( this);
 
        // количество строк
        gridLayout.setRowCount(3);
        // количество столбцов
        gridLayout.setColumnCount(3);
 
        for(int i = 1; i <=3; i++){
            Button btn = new Button(this);
            btn.setText(String.valueOf(i));
            gridLayout.addView(btn);
        }
 
        Button btn4 = new Button(this);
        btn4.setText("4");
        GridLayout.LayoutParams layoutParams4 = new GridLayout.LayoutParams();
        layoutParams4.columnSpec = GridLayout.spec(0,2);
        layoutParams4.width = (int) TypedValue.applyDimension(
                TypedValue.COMPLEX_UNIT_DIP, 180, getResources().getDisplayMetrics());
        gridLayout.addView(btn4, layoutParams4);
 
 
        Button btn5 = new Button(this);
        btn5.setText("5");
        GridLayout.LayoutParams layoutParams5 = new GridLayout.LayoutParams();
        layoutParams5.rowSpec = GridLayout.spec(1,2);
        layoutParams5.height = (int) TypedValue.applyDimension(
                TypedValue.COMPLEX_UNIT_DIP, 100, getResources().getDisplayMetrics());
        gridLayout.addView(btn5, layoutParams5);
 
        Button btn6 = new Button(this);
        btn6.setText("6");
        Button btn7 = new Button(this);
        btn7.setText("7");
        gridLayout.addView(btn6);
        gridLayout.addView(btn7);
         
        setContentView(gridLayout);
    }
}
```

## 2.15 Java и Android | ScrollView

Контейнер ScrollView предназначен для создания прокрутки для такого интерфейса, все элементы которого одномоментно не могут поместиться на экране устройства. ScrollView может вмещать только один элемент, поэтому если мы хотим разместить несколько элементов, то их надо поместить в какой-нибудь контейнер.

Например, определим ряд TextView с большими текстами:

```java
<ScrollView
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:orientation="vertical"
        >
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="What is Lorem Ipsum?"
            android:textSize="34sp" />
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Lorem Ipsum is simply dummy text of the printing and typesetting industry...like Aldus PageMaker including versions of Lorem Ipsum."
            android:textSize="14sp"/>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Why do we use it?"
            android:layout_marginTop="16dp"
            android:textSize="34sp"/>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Lorem Ipsum is simply dummy text of the printing and typesetting industry...like Aldus PageMaker including versions of Lorem Ipsum."
            android:textSize="14sp"/>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Where can I get some?"
            android:layout_marginTop="16dp"
            android:textSize="34sp"/>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="There are many variations of passages of Lorem Ipsum available ... or non-characteristic words etc."
            android:textSize="14sp"/>
    </LinearLayout>
</ScrollView>
```

Так как в ScrollView можно поместить только один элемент, то все TextView заключены в LinearLayout. И если площадь экрана будет недостаточной, чтобы поместить все содержимое LinearLayout, то станет доступной прокрутка:

Создание ScrollView программно в коде MainActivity:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.view.ViewGroup;
import android.widget.ScrollView;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        //setContentView(R.layout.activity_main);
 
        ScrollView scrollView = new ScrollView(this);
 
        TextView textView = new TextView(this);
        textView.setText("Lorem Ipsum is simply dummy text of the printing and typesetting industry...like Aldus PageMaker including versions of Lorem Ipsum.");
        textView.setLayoutParams(new ViewGroup.LayoutParams
                (ViewGroup.LayoutParams.WRAP_CONTENT, ViewGroup.LayoutParams.WRAP_CONTENT));
        textView.setTextSize(26);
        scrollView.addView(textView);
        setContentView(scrollView);
    }
}
```

## 2.16 Java и Android | Вложенные layout

Одна layout может содержать другую layout. Для этого применяется элемент include.

Например, добавим в папку res/layout два файла layout, которые пусть будут называться text_panel.xml и button_panel.xml:

В файле text_panel.xml определим следующий код:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content">
    <TextView
        android:id="@+id/clicksText"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="30sp"
        android:text="0 Clicks"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        />
</androidx.constraintlayout.widget.ConstraintLayout>
```

По сути здесь просто определено поле TextView для вывода текста.

В файле button_panel.xml определим следующую разметку:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content">
    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Click"
        android:onClick="onClick"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Здесь определена кнопка, нажатия которой мы будем обрабатывать.

Основным файлом разметки, который определяет интерфейс приложения, по-прежнему является activity_main.xml. Изменим его:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="16dp"
    tools:context=".MainActivity">
 
    <include
        android:id="@+id/textView"
        layout="@layout/text_panel"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintBottom_toTopOf="@+id/button"
        />
    <include
        android:id="@+id/button"
        layout="@layout/button_panel"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView"
        />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

С помощью ConstraintLayout весь интерфейс здесь организуется в виде вертикального стека. С помощью элементов include внутрь ConstraintLayout добавляется содержимое файлов text_panel.xml и button_panel.xml. Для указания названия файла применяется атрибут layout.

Это все равно, что если бы мы напрямую вместо элемента include добавили содержимое файлов. Однако такой способ имеет свои преимущества. Например, какая-то часть разметки, группа элементов управления может повторяться в различных activity. И чтобы не определять по сто раз эти элементы, можно вынести их в отдельный файл layout и с помощью include подключать их.

После добавления в ConstraintLayout к элементам include можно применять все те стандартные атрибуты, которые применяются в этом контейнере к вложенным элементам, например, настроить размеры, расположение. Также стоит отметить, что добавлять внешние layout можно не только в ConstraintLayout, но и в другие контейнеры (LinearLayout, RelativeLayout и т.д.)

Также изменим код MainActivity:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.view.View;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    int clicks = 0;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
 
    public void onClick(View view){
        TextView clicksText = findViewById(R.id.clicksText);
        clicks++;
        clicksText.setText(clicks + " Clicks");
    }
}
```

В MainActivity мы можем обращаться к элементам во вложенных файлах layout. Например, мы можем установить обработчик нажатия кнопки, в котором при нажатии изменять текст в TextView.

При этом мы несколько раз можем добавлять в один файл layout другой файл layout. Для этого вначале изменим файл button_panel.xml следующим образом:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:background="#3F51B5"
    android:paddingTop="10dp"
    android:paddingBottom="10dp">
    <Button
        android:id="@+id/clickBtn"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

И изменим файл activity_main.xml:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="16dp"
    tools:context=".MainActivity">
 
    <include
        layout="@layout/text_panel"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        />
    <include layout="@layout/button_panel"
        android:id="@+id/plus_button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintRight_toLeftOf="@+id/minus_button"/>
 
    <include layout="@layout/button_panel"
        android:id="@+id/minus_button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginLeft="36dp"
        app:layout_constraintLeft_toRightOf="@id/plus_button"
        app:layout_constraintBottom_toBottomOf="parent"/>
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Теперь файл button_panel.xml добавляется два раза. Важно, что при добавлении этого файла каждому элементу include присвоен определенный id. По этому id мы сможем узнать, о каком именно элементе include идет речь.

Также изменим MainActivity:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    int clicks = 0;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
 
        View plusButtonView = findViewById(R.id.plus_button);
        View minusButtonView = findViewById(R.id.minus_button);
        TextView clicksText = findViewById(R.id.clicksText);
 
        Button plusButton = plusButtonView.findViewById(R.id.clickBtn);
        Button minusButton = minusButtonView.findViewById(R.id.clickBtn);
 
        plusButton.setText("+");
        minusButton.setText("-");
 
        plusButton.setOnClickListener(v -> {
            clicks++;
            clicksText.setText(clicks + " Clicks");
        });
        minusButton.setOnClickListener(v -> {
            clicks--;
            clicksText.setText(clicks + " Clicks");
        });
    }
}
```

Здесь вначале мы получаем отдельные элементы include по id. Затем в рамках этих элементов получаем кнопку. После этого мы можем установить у кнопко любой текст и повесить обработчик события нажатия. И таким образом, поведение обеих кнопок будет различаться.

## 2.17 Java и Android | Gravity и позиционирование внутри элемента

Атрибут gravity задает позиционирование содержимого внутри визуального элемента. Он может принимать следующие значения:

-    top: элементы размещаются вверху

-    bottom: элементы размещаются внизу

-    left: элементы размещаются в левой стороне

-    right: элементы размещаются в правой стороне контейнера

-    center_vertical: выравнивает элементы по центру по вертикали

-    center_horizontal: выравнивает элементы по центру по горизонтали

-    center: элементы размещаются по центру

-    fill_vertical: элемент растягивается по вертикали

-    fill_horizontal: элемент растягивается по горизонтали

-    fill: элемент заполняет все пространство контейнера

-    clip_vertical: обрезает верхнюю и нижнюю границу элементов

-    clip_horizontal: обрезает правую и левую границу элементов

-    start: элемент позиционируется в начале (в верхнем левом углу) контейнера

-    end: элемент позиционируется в конце контейнера(в верхнем правом углу)

Например, поместим текст в самый низ в элементе TextView:

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
        android:gravity="bottom"
         
        android:layout_width="0dp"
        android:layout_height="200dp"
        android:text="Hello Android!"
        android:textSize="30sp"
        android:background="#e8eaf6"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

При необходимости мы можем комбинировать значения, разделяя их вертикальной чертой:

```java
<TextView
    android:gravity="bottom|right"
         
    android:layout_width="0dp"
    android:layout_height="200dp"
    android:text="Hello Android!"
    android:textSize="30sp"
    android:background="#e8eaf6"
    app:layout_constraintLeft_toLeftOf="parent"
    app:layout_constraintRight_toRightOf="parent"
    app:layout_constraintTop_toTopOf="parent" />
```

### Программная установка gravity

Чтобы установить параметр gravity у элемента надо вызвать метод setGravity(). В качестве параметра в метод передается одна из констант класса Gravity, которые аналогичны значениям атрибута (за тем исключенем, что названия в верхнем регистре):

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import androidx.constraintlayout.widget.ConstraintLayout;
 
import android.os.Bundle;
import android.view.Gravity;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
 
        ConstraintLayout constraintLayout = new ConstraintLayout(this);
        TextView textView = new TextView(this);
        textView.setText("Hello Android!");
        textView.setTextSize(30);
        textView.setBackgroundColor(0xffe8eaf6);
 
        // установка gravity
        textView.setGravity(Gravity.CENTER);
 
        // установка высоты и ширины
        ConstraintLayout.LayoutParams layoutParams = new ConstraintLayout.LayoutParams
                (ConstraintLayout.LayoutParams.MATCH_CONSTRAINT, 200);
        layoutParams.leftToLeft = ConstraintLayout.LayoutParams.PARENT_ID;
        layoutParams.rightToRight = ConstraintLayout.LayoutParams.PARENT_ID;
        layoutParams.topToTop = ConstraintLayout.LayoutParams.PARENT_ID;
        layoutParams.bottomToBottom = ConstraintLayout.LayoutParams.PARENT_ID;
        textView.setLayoutParams(layoutParams);
 
        constraintLayout.addView(textView);
        setContentView(constraintLayout);
    }
}
```

Для сочетания нескольких значений также можно использовать вертикальную черту:

```java
textView.setGravity(Gravity.BOTTOM | Gravity.CENTER);
```

# Глава 3. Основные элементы управления

## 3.1 Java и Android | TextView

Для простого вывода текста на экран предназначен элемент TextView. Он просто отображает текст без возможности его редактирования. Некоторые его основные атрибуты:

-    android:text: устанавливает текст элемента

-    android:textSize: устанавливает высоту текста, в качестве единиц измерения для указания высоты используются sp

-    android:background: задает фоновый цвет элемента в виде цвета в шестнадцатиричной записи или в виде цветового ресурса

-    android:textColor: задает цвет текста

-    android:textAllCaps: при значении true делает все символы в тексте заглавными

-    android:textDirection: устанавливает направление текста. По умолчанию используется направление слева направо, но с помощью значения rtl можно установить направление справо налево

-    android:textAlignment: задает выравнивание текста. Может принимать следующие значения:

     -   center: выравнивание по центру

     -   textStart: по левому краю

     -   textEnd: по правому краю

     -   viewStart: при направлении текста слева направо выравнивание по левому краю, при направлении справа налево - по правому

     -   viewEnd: при направлении текста слева направо выравнивание по правому краю, при направлении справа налево - по левому

-    android:fontFamily: устанавливает тип шрифта. Может принимать следующие значения:

      -  monospace

      -  serif

     -  serif-monospace

     -  sans-serif

     -  sans-serif-condensed

     - sans-serif-smallcaps

     - sans-serif-light

     -  casual
 
     -  cursive

     -  cursive

Например, определим три текстовых поля:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
 
    <TextView
        android:layout_height="wrap_content"
        android:layout_width="0dp"
        android:layout_margin="10dp"
 
        android:text="Hello Android "
        android:fontFamily="sans-serif"
        android:textSize="26sp"
        android:background="#ffebee"
        android:textColor="#f44336"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintRight_toRightOf="parent"/>
    <TextView
        android:layout_height="wrap_content"
        android:layout_width="0dp"
        android:layout_margin="10dp"
 
        android:text="Hello Java"
        android:textAllCaps="true"
        android:textSize="26sp"
        android:background="#ede7f6"
        android:textColor="#7e57c2"
 
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintRight_toRightOf="parent"/>
 
    <TextView
        android:layout_height="wrap_content"
        android:layout_width="0dp"
        android:layout_margin="10dp"
 
        android:text="Hello World"
        android:textAlignment="textEnd"
        android:textSize="26sp"
        android:background="#e8eaf6"
        android:textColor="#5c6bc0"
         
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintRight_toRightOf="parent"/>
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Установка элемента в коде тоже не отличается сложностью. Например, создадим элемент и выведем его на экран:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import androidx.constraintlayout.widget.ConstraintLayout;
 
import android.graphics.Typeface;
import android.os.Bundle;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
 
        ConstraintLayout constraintLayout = new ConstraintLayout(this);
        TextView textView = new TextView(this);
        // установка фонового цвета
        textView.setBackgroundColor(0xffe8eaf6);
        // установка цвета текста
        textView.setTextColor(0xff5c6bc0);
        // делаем все буквы заглавными
        textView.setAllCaps(true);
        // устанавливаем вравнивание текста по центру
        textView.setTextAlignment(TextView.TEXT_ALIGNMENT_CENTER);
        // устанавливаем текста
        textView.setText("Hello Android!");
        // установка шрифта
        textView.setTypeface(Typeface.create("casual", Typeface.NORMAL));
        // устанавливаем высоту текста
        textView.setTextSize(26);
 
        ConstraintLayout.LayoutParams layoutParams = new ConstraintLayout.LayoutParams
                (ConstraintLayout.LayoutParams.WRAP_CONTENT, ConstraintLayout.LayoutParams.WRAP_CONTENT);
        layoutParams.leftToLeft = ConstraintLayout.LayoutParams.PARENT_ID;
        layoutParams.topToTop = ConstraintLayout.LayoutParams.PARENT_ID;
        textView.setLayoutParams(layoutParams);
 
        constraintLayout.addView(textView);
        setContentView(constraintLayout);
    }
}
```

Иногда необходимо вывести на экран какую-нибудь ссылку, либо телефон, по нажатию на которые производилось бы определенное действие. Для этого в TextView определен атрибут android:autoLink:

```java
<TextView
    android:text="Посетите сайт https://metanit.com"
    android:textSize="21sp"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:autoLink="web|email"
     
    app:layout_constraintLeft_toLeftOf="parent"
    app:layout_constraintTop_toTopOf="parent"/>
```

- android:autoLink может принимать несколько значений:

  -   none: отключает все ссылки
 
  -   web: включает все веб-ссылки

  -   email: включает ссылки на электронные адреса

   -  phone: включает ссылки на номера телефонов

   -  map: включает ссылки на карту

   -  all: включает все вышеперечисленные ссылки

То есть при настройке android:autoLink="web" если в тексте есть упоминание адреса url, то этот адрес будет выделяться, а при нажатии на него будет осуществлен переход к веб-браузеру, который откроет страницу по этому адресу. С помощью прямой черты мы можем объединять условия, как в данном случае: android:autoLink="web|email"

## 3.2 Java и Android | EditText

Элемент EditText является подклассом класса TextView. Он также представляет текстовое поле, но теперь уже с возможностью ввода и редактирования текста. Таким образом, в EditText мы можем использовать все те же возможности, что и в TextView.

Из тех атрибутов, что не рассматривались в теме про TextView, следует отметить атрибут android:hint. Он позволяет задать текст, который будет отображаться в качестве подсказки, если элемент EditText пуст. Кроме того, мы можем использовать атрибут android:inputType, который позволяет задать клавиатуру для ввода. В частности, среди его значений можно выделить следующие:

-    text: обычная клавиатура для ввода однострочного текста

-    textMultiLine: многострочное текстовое поле

-    textEmailAddress: обычная клавиатура, на которой присутствует символ @, ориентирована на ввод email

-    textUri: обычная клавиатура, на которой присутствует символ /, ориентирована на ввод интернет-адресов

-    textPassword: клавиатура для ввода пароля

-    textCapWords: при вводе первый введенный символ слова представляет заглавную букву, остальные - строчные

 -   number: числовая клавиатура

-    phone: клавиатура в стиле обычного телефона

-    date: клавиатура для ввода даты

-    time: клавиатура для ввода времени

-    datetime: клавиатура для ввода даты и времени

Используем EditText:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
 
    <EditText
        android:id="@+id/name"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:hint="Введите имя"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintRight_toRightOf="parent"/>
    <EditText
        android:id="@+id/message"
        android:layout_marginTop="16dp"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:hint="Введите сообщение"
        android:inputType="textMultiLine"
        android:gravity="top"
        app:layout_constraintTop_toBottomOf="@+id/name"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintBottom_toBottomOf="parent" />
     
</androidx.constraintlayout.widget.ConstraintLayout>
```

Первое поле здесь обычное однострочное, а второе - многострочное. Чтобы во втором поле текст выравнивался по верху, дополнительно устанавливается атрибут android:gravity="top"

Одной из возможностей элемента EditText также является возможность обработать введенные символы по мере ввода пользователя. Для этого определим в файле activity_main.xml следующую разметку:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
 
    <TextView
        android:id="@+id/textView"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:textSize="34sp"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"/>
    <EditText
        android:id="@+id/editText"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:hint="Введите имя"
        app:layout_constraintTop_toBottomOf="@+id/textView"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent" />
 
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Предполагается, что введенные в EditText символы тут же будут отображаться в элементе TextView. И для этого также изменим код MainActivity:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.text.Editable;
import android.text.TextWatcher;
import android.widget.EditText;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
 
        EditText editText = findViewById(R.id.editText);
 
        editText.addTextChangedListener(new TextWatcher() {
 
            public void afterTextChanged(Editable s) {}
 
            public void beforeTextChanged(CharSequence s, int start,
                                          int count, int after) {
            }
 
            public void onTextChanged(CharSequence s, int start, int before, int count) {
                TextView textView = findViewById(R.id.textView);
                textView.setText(s);
            }
        });
    }
}
```

С помощью метода addTextChangedListener() здесь к элементу EditText добавляется слушатель ввода текста - объект TextWatcher. Для его использования нам надо реализовать три метода, но в реальности нам хватит реализации метода onTextChanged, который вызывается при изменении текста. Введенный текст передается в этот метод в качестве параметра CharSequence. В самом методе просто передаем этот текст в элемент TextView.

В итоге при вводе в EditText все символы также будут отображаться в TextView.

## 3.3 Java и Android | Button 

Одним из часто используемых элементов являются кнопки, которые представлены классом android.widget.Button. Ключевой особенностью кнопок является возможность взаимодействия с пользователем через нажатия.

Некоторые ключевые атрибуты, которые можно задать у кнопок:

-    text: задает текст на кнопке

-    textColor: задает цвет текста на кнопке

 -   background: задает фоновый цвет кнопки

-    textAllCaps: при значении true устанавливает текст в верхнем регистре. По умолчанию как раз и применяется значение true

-    onClick: задает обработчик нажатия кнопки

Итак, изменим код в activity_main.xml следующим образом:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
 
    <TextView
        android:id="@+id/textView"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:textSize="34sp"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"/>
    <EditText
        android:id="@+id/editText"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:hint="Введите имя"
        app:layout_constraintTop_toBottomOf="@+id/textView"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent" />
    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Ввод"
        android:onClick="sendMessage"
        app:layout_constraintTop_toBottomOf="@+id/editText"
        app:layout_constraintLeft_toLeftOf="parent" />
 
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

При помощью атрибута android:onClick можно задать метод в коде java, который будет обрабатывать нажатия кнопки. Так, в вышеприведенном примере это метод sendMessage. Теперь перейдем к коду MainActivity и пропишем в нем такой метод:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
    // Обработка нажатия кнопки
    public void sendMessage(View view) {
        TextView textView = findViewById(R.id.textView);
        EditText editText = findViewById(R.id.editText);
        textView.setText("Добро пожаловать, " + editText.getText());
    }
}
```

При создании метода обработки нажатия следует учитывать следующие моменты:

 -   Метод должен объявляться с модификатором public

 -   Должен возвращать значение void

  -  В качестве параметра принимать объект View. Этот объект View и представляет собой нажатую кнопку

В данном случае после нажатия на кнопку в TextView выводится текст из EditText.

Аналогичный пример полностью в коде MainActivity:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import androidx.constraintlayout.widget.ConstraintLayout;
 
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    EditText editText;
    TextView textView;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        //setContentView(R.layout.activity_main);
 
        ConstraintLayout constraintLayout = new ConstraintLayout(this);
        textView = new TextView(this);
        textView.setId(View.generateViewId());
        ConstraintLayout.LayoutParams textViewLayout =  new ConstraintLayout.LayoutParams(
                ConstraintLayout.LayoutParams.MATCH_CONSTRAINT, ConstraintLayout.LayoutParams.WRAP_CONTENT
        );
        textViewLayout.topToTop = ConstraintLayout.LayoutParams.PARENT_ID;
        textViewLayout.leftToLeft = ConstraintLayout.LayoutParams.PARENT_ID;
        textViewLayout.rightToRight = ConstraintLayout.LayoutParams.PARENT_ID;
        textView.setLayoutParams(textViewLayout);
        constraintLayout.addView(textView);
 
        editText = new EditText(this);
        editText.setId(View.generateViewId());
        editText.setHint("Введите имя");
        ConstraintLayout.LayoutParams editTextLayout =  new ConstraintLayout.LayoutParams(
                ConstraintLayout.LayoutParams.MATCH_CONSTRAINT, ConstraintLayout.LayoutParams.WRAP_CONTENT
        );
        editTextLayout.topToBottom = textView.getId();
        editTextLayout.leftToLeft = ConstraintLayout.LayoutParams.PARENT_ID;
        editTextLayout.rightToRight = ConstraintLayout.LayoutParams.PARENT_ID;
        editText.setLayoutParams(editTextLayout);
        constraintLayout.addView(editText);
 
        Button button = new Button(this);
        button.setText("Ввод");
        ConstraintLayout.LayoutParams buttonLayout =  new ConstraintLayout.LayoutParams(
                ConstraintLayout.LayoutParams.WRAP_CONTENT, ConstraintLayout.LayoutParams.WRAP_CONTENT
        );
        buttonLayout.topToBottom = editText.getId();
        buttonLayout.leftToLeft = ConstraintLayout.LayoutParams.PARENT_ID;
        button.setLayoutParams(buttonLayout);
        constraintLayout.addView(button);
 
        button.setOnClickListener(new View.OnClickListener() {
            public void onClick(View v) {
                // Обработка нажатия
                textView.setText("Добро пожаловать, " + editText.getText());
            }
        });
 
        setContentView(constraintLayout);
    }
}
```

При программном создании кнопки мы можем определить у нее слушатель нажатия View.OnClickListener и с помощью его метода onClick также обработать нажатие:

```java
button.setOnClickListener(new View.OnClickListener() {
    public void onClick(View v) {
        // Обработка нажатия
    }
});
```

## 3.4 Java и Android | Приложение Калькулятор

Зная некоторые основы компоновки и такие элементы как TextView, EditText и Button, уже можно составить более менее полноценное приложение. В данном случае мы сделаем простенький калькулятор.

Для этого создадим новый проект и определим в файле activity_main.xml следующий интерфейс:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="8dp">
    <!-- поле результата -->
    <TextView
        android:id="@+id/resultField"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        app:layout_constraintHorizontal_weight="1"
        android:textSize="18sp"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toLeftOf="@+id/operationField"/>
    <!-- поле знака операции -->
    <TextView
        android:id="@+id/operationField"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        app:layout_constraintHorizontal_weight="1"
        android:textSize="18sp"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintLeft_toRightOf="@+id/resultField"
        />
    <!-- поле ввода чисел -->
    <EditText
        android:id="@+id/numberField"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:inputType="phone"
        app:layout_constraintTop_toBottomOf="@+id/resultField"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"/>
 
    <LinearLayout
        android:id="@+id/firstButtonPanel"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginTop="16dp"
        app:layout_constraintTop_toBottomOf="@+id/numberField"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent">
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="7"
            android:id="@+id/n7" />
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="8"
            android:id="@+id/n8"/>
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="9"
            android:id="@+id/n9"/>
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="/"
            android:id="@+id/div"/>
    </LinearLayout>
    <LinearLayout
        android:id="@+id/secondButtonPanel"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginTop="16dp"
        app:layout_constraintTop_toBottomOf="@+id/firstButtonPanel"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent">
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="4"
            android:id="@+id/n4"/>
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="5"
            android:id="@+id/n5"/>
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="6"
            android:id="@+id/n6"/>
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="*"
            android:id="@+id/mul"/>
    </LinearLayout>
    <LinearLayout
        android:id="@+id/thirdButtonPanel"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginTop="16dp"
        app:layout_constraintTop_toBottomOf="@+id/secondButtonPanel"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent">
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="1"
            android:id="@+id/n1"/>
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="2"
            android:tag="num"
            android:id="@+id/n2"/>
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="3"
            android:id="@+id/n3"/>
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="-"
            android:id="@+id/sub" />
    </LinearLayout>
    <LinearLayout
        android:id="@+id/forthButtonPanel"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginTop="16dp"
        app:layout_constraintTop_toBottomOf="@+id/thirdButtonPanel"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent">
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="0"
            android:id="@+id/n0"/>
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text=","
            android:id="@+id/comma"/>
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="+"
            android:id="@+id/add"/>
        <Button
            android:layout_weight="1"
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:text="="
            android:id="@+id/eq"/>
    </LinearLayout>
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

В итоге весь интерфейс будет выглядеть следующим образом:

Корневой контейнер компоновки представляет элемент ConstraintLayout . Сверху в нем определены два текстовых поля TextView: одно для вывода результата вычислений и одно для вывода текущего знака операции.

Затем идет элемент EditText, предназначенный для ввода чисел.

И далее расположены четыре элемента LinearLayout с горизонтальными рядами кнопок. Чтобы все кнопки занимали равное пространство внутри контейнера, для них установлены атрибуты android:layout_weight="1" и android:layout_width="0dp".

Для каждой кнопки установлен идентификатор, чтобы в коде можно было прикрепить к ней определенный обработчик нажатия.

Теперь изменим класс MainActivity:

```java
package com.metanit.calculator;
 
import androidx.annotation.NonNull;
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.widget.EditText;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    TextView resultField; // текстовое поле для вывода результата
    EditText numberField;   // поле для ввода числа
    TextView operationField;    // текстовое поле для вывода знака операции
    Double operand = null;  // операнд операции
    String lastOperation = "="; // последняя операция
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        // получаем все поля по id из activity_main.xml
        resultField = findViewById(R.id.resultField);
        numberField = findViewById(R.id.numberField);
        operationField = findViewById(R.id.operationField);
 
        findViewById(R.id.add).setOnClickListener((view)->onOperationClick("+"));
        findViewById(R.id.sub).setOnClickListener((view)->onOperationClick("-"));
        findViewById(R.id.mul).setOnClickListener((view)->onOperationClick("*"));
        findViewById(R.id.div).setOnClickListener((view)->onOperationClick("/"));
        findViewById(R.id.eq).setOnClickListener((view)->onOperationClick("="));
 
        findViewById(R.id.n0).setOnClickListener((view)->onNumberClick("0"));
        findViewById(R.id.n1).setOnClickListener((view)->onNumberClick("1"));
        findViewById(R.id.n2).setOnClickListener((view)->onNumberClick("2"));
        findViewById(R.id.n3).setOnClickListener((view)->onNumberClick("3"));
        findViewById(R.id.n4).setOnClickListener((view)->onNumberClick("4"));
        findViewById(R.id.n5).setOnClickListener((view)->onNumberClick("5"));
        findViewById(R.id.n6).setOnClickListener((view)->onNumberClick("6"));
        findViewById(R.id.n7).setOnClickListener((view)->onNumberClick("7"));
        findViewById(R.id.n8).setOnClickListener((view)->onNumberClick("8"));
        findViewById(R.id.n9).setOnClickListener((view)->onNumberClick("9"));
        findViewById(R.id.comma).setOnClickListener((view)->onNumberClick(","));
    }
    // сохранение состояния
    @Override
    protected void onSaveInstanceState(Bundle outState) {
        outState.putString("OPERATION", lastOperation);
        if(operand!=null)
            outState.putDouble("OPERAND", operand);
        super.onSaveInstanceState(outState);
    }
    // получение ранее сохраненного состояния
    @Override
    protected void onRestoreInstanceState(@NonNull Bundle savedInstanceState) {
        super.onRestoreInstanceState(savedInstanceState);
        lastOperation = savedInstanceState.getString("OPERATION");
        operand= savedInstanceState.getDouble("OPERAND");
        resultField.setText(operand.toString());
        operationField.setText(lastOperation);
    }
    // обработка нажатия на числовую кнопку
    public void onNumberClick(String number){
        numberField.append(number);
        if(lastOperation.equals("=") && operand!=null){
            operand = null;
        }
    }
    // обработка нажатия на кнопку операции
    public void onOperationClick(String op){
 
        String number = numberField.getText().toString();
        // если введенно что-нибудь
        if(number.length()>0){
            number = number.replace(',', '.');
            try{
                performOperation(Double.valueOf(number), op);
            }catch (NumberFormatException ex){
                numberField.setText("");
            }
        }
        lastOperation = op;
        operationField.setText(lastOperation);
    }
 
    private void performOperation(Double number, String operation){
 
        // если операнд ранее не был установлен (при вводе самой первой операции)
        if(operand ==null){
            operand = number;
        }
        else{
            if(lastOperation.equals("=")){
                lastOperation = operation;
            }
            switch(lastOperation){
                case "=":
                    operand =number;
                    break;
                case "/":
                    if(number==0){
                        operand =0.0;
                    }
                    else{
                        operand /=number;
                    }
                    break;
                case "*":
                    operand *=number;
                    break;
                case "+":
                    operand +=number;
                    break;
                case "-":
                    operand -=number;
                    break;
            }
        }
        resultField.setText(operand.toString().replace('.', ','));
        numberField.setText("");
    }
}
```

Разберем этот код. Вначале в методе onCreate() получаем все поля из activity_main.xml, текст которых будет изменяться:

```java
resultField = findViewById(R.id.resultField);
numberField = findViewById(R.id.numberField);
operationField = findViewById(R.id.operationField);
```

Далее для каждой кнопки назначаем определенный обработчик нажатия - в зависимости от типа кнопки это либо метод onNumberClick, в который передается нажатое число, либо onOperationClick, в который передается знак операции.

Результат операции будет попадать в переменную operand, которая представляет тип Double, а знак операции - в переменную lastOperation:

```java
Double operand = null;
String lastOperation = "=";
```

Так как при переходе от портретной ориентации к альбомной или наоборот мы можем потерять все введенные данные, то чтобы их не потерять, мы их сохраняем в методе onSaveInstanceState() и обратно получаем в методе onRestoreInstanceState().

При нажатии на числовую кнопку будет вызываться метод onNumberClick, в котором добавляем введенную цифру или знак запятой к тексту в поле numberField:

```java
numberField.append(number);
 
if(lastOperation.equals("=") && operand!=null){
    operand = null;
}
```

При этом если последняя операция представляла собой получение результата (знак "равно"), то мы сбрасываем переменную operand.

В методе onOperationClick происходит обработка нажатия на кнопку со знаком операции:

```java
String number = numberField.getText().toString();
if(number.length()>0){
    number = number.replace(',', '.');
    try{
        performOperation(Double.valueOf(number), op);
    }catch (NumberFormatException ex){
        numberField.setText("");
    }
}
lastOperation = op;
operationField.setText(lastOperation);
```

Здесь получаем ранее введенное число и введенную операцию и передаем их в метод performOperation(). Так как в метод передается не просто строка, а число Double, то нам надо преобразовать строку в чсло. И поскольку теоретически могут быть введены нечисловые символы, то для отлова исключения, которое может возникнуть при преобразовании используется конструкция try...catch.

Кроме того, так как разделителем целой и дробной части в Double в java является точка, то нам надо заменить запятую на точку, так как предполагается, что мы используем в качестве разделителя запятую.

А методе performOperation() выполняем собственно операцию. При вводе первой операции, когда операнд еще не установлен, мы просто устанавливаем операнд:

```java
if(operand ==null){
    operand = number;
}
```

При вводе второй и последующих операций применяем предыдущую операцию, знак которой хранится в переменной lastOperation, к операнду operand и второму числу, которое было введено в числовое поле. Полученный результат операции сохраняем в переменной operand.

## 3.5 Java и Android | Всплывающие окна. Toast

Для создания простых уведомлений в Android используется класс Toast. Фактически Toast представляет всплывающее окно с некоторым текстом, которое отображается в течение некоторого времени.

Объект Toast нельзя создать в коде разметки xml, например, в файл activity_main.xml. Toast можно использовать только в коде java.

Так, определим в файле разметки activity_main.xml кнопку:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="16dp">
 
    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Click"
        android:onClick="onClick"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

У кнопки установлен обработчик нажатия - метод onClick. Определим его в коде MainActivity:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.view.View;
import android.widget.Toast;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
 
        setContentView(R.layout.activity_main);
    }
 
    public  void onClick(View view){
        Toast toast = Toast.makeText(this, "Hello Android!",Toast.LENGTH_LONG);
        toast.show();
    }
}
```

В обработчике отображается всплывающее окно. Для его создания применяется метод Toast.makeText(), в который передается три параметра: текущий контекст (текущий объект activity), отображаемый текст и время отобажения окна.

В качестве времени показа окна мы можем использовать целочисленное значение - колическо миллисекунд или встроенные константы Toast.LENGTH_LONG (3500 миллисекунд) и Toast.LENGTH_SHORT (2000 миллисекунд).

Для самого отображения окна вызывается метод show():

По умолчанию окно отображается внизу интерфейса с центрированием по центру. Но мы можем кастомизировать позиционирование окна с помощью методов setGravity() и setMargin(). Так, изменим метод onClick:

```java
public  void onClick(View view){
     
    Toast toast = Toast.makeText(this, "Hello Android!", Toast.LENGTH_LONG);
    toast.setGravity(Gravity.TOP, 0,160);   // import android.view.Gravity;
    toast.show();
}
```

Первый параметр метода setGravity указывает, в какой части контейнера надо позиционировать Toast, второй и третий параметр устанавливают отступы от этой позиции по горизонтали и вертикали сооветственно:

Метод setMargin() принимает два параметра: отступ от левой границы контейнера в процентах от шиирины контейнера и отступ от верхней границы в процентах от длины контейнера.

## 3.6 Java и Android | Snackbar

Элемент Snackbar в некотором роде похож на Toast: он также позволяет выводить всплывающие сообщения, но теперь сообщения растягиваются по ширине экрана.

Для применения Snackbar добавим в файл activity_main.xml определение кнопки, по нажатию на которую будет появляться Snackbar:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="16dp">
 
    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Click"
        android:onClick="onClick"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Здесь определена кнопка, по нажатию на которую будет оображаться сообщение.

И также изменим класс MainActivity:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
 
import com.google.android.material.snackbar.Snackbar;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
 
    public  void onClick(View view){
        Snackbar.make(view, "Hello Android", Snackbar.LENGTH_LONG)
                .show();
    }
}
```

Snackbar создается с помощью метода make(), в который передаются три параметра: объект View, к которому прикрепляется всплывающее ообщение, само сообщение в виде строки и параметр, который указывает, сколько будет отображаться сообщение. Последний параметр может принимать числовое значение - количество миллисекунд, либо одну из трех констант: Snackbar.LENGTH_INDEFINITE (отображение в течение неопределенного периода времени), Snackbar.LENGTH_LONG (долгое отображение) или Snackbar.LENGTH_SHORT (недолгое отображение).

После создания Snackbar отображается с помощью метода show:

При этом в отличие от Toast мы не можем повлиять на позицию сообщения, оно отображается внизу экрана и занимает всю нижнюю часть.

### Прикрепление обработчика события

Snackbar позволяет добавить виджету действие, чтобы пользователь мог как-то прореагировать на сообщение. Например, изменим код MainActivity следующим образом:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.Toast;
 
import com.google.android.material.snackbar.Snackbar;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
 
    public  void onClick(View view){
        Snackbar snackbar = Snackbar.make(view, "Hello Android", Snackbar.LENGTH_LONG);
         
        snackbar.setAction("Next...", new View.OnClickListener (){
            @Override
            public void onClick(View v) {
                Toast toast = Toast.makeText(getApplicationContext(), "Next clicked!",Toast.LENGTH_LONG);
                toast.show();
            }
        });
        snackbar.show();
    }
}
```

Для добавления действия у Snackbar применяется метод setAction(). Первый параметр представляет текст кнопки в сообщении, на которую может нажать пользователь - в данном случае это "Next...". Второй параметр представляет реализацию интерфейса View.OnClickListener (тот же самый, который используется для обработки нажатия кнопки). В методе onClick() сообственно выполняем действия, которые вызываются при нажатии на кнопку в сообщении. В данном случае для простоты просто отображаем всплывающее сообщение в виде объекта Toast

### Настройка визуального вида

Ряд методов Snackbar позволяет настроить внешний вид:

  -  setTextColor(): настраивает цвет текста

  -  setBackgroundTint(): настраивает цвет фона

  -  setActionTextColor(): настраивает цвет текста кнопки в всплывающем сообщении

```java
snackbar.setTextColor(0XFF81C784);
snackbar.setBackgroundTint(0XFF555555);
snackbar.setActionTextColor(0XFF0277BD);
```

## 3.7 Java и Android | Checkbox

Элементы Checkbox представляют собой флажки, которые могут находиться в отмеченном и неотмеченном состоянии. Флажки позволяют производить множественный выбор из нескольких значений. Итак, определим в файле разметки activity_main.xml элемент CheckBox:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="16dp">
 
    <TextView android:id="@+id/selection"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="26sp"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"/>
 
    <CheckBox android:id="@+id/enabled"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Включить"
        android:textSize="26sp"
 
        android:onClick="onCheckboxClicked"
 
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/selection"/>
 
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Атрибут android:onClick, как и в случае с простыми кнопками, позволяет задать обработчик нажатия на флажок. Определим обработчик нажатия в коде MainActivity:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.view.View;
import android.widget.CheckBox;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
 
    public void onCheckboxClicked(View view) {
        // Получаем флажок
        CheckBox checkBox = (CheckBox) view;
        TextView selection = findViewById(R.id.selection);
        // Получаем, отмечен ли данный флажок
        if(checkBox.isChecked()) {
            selection.setText("Включено");
            checkBox.setText("Выключить");
        }
        else {
            selection.setText("Выключено");
            checkBox.setText("Включить");
        }
    }
}
```

В качестве параметра в обработчик нажатия onCheckboxClicked передается нажатый флажок. Обработчик срабатывает при каждом нажатии на checkBox. То есть и когда мы устанавливаем флажок, и когда мы снимем отметку. С помощью метода isChecked() можно узнать, выделен ли флажок - в этом случае метод возвращает true.

Подобным образом можно использовать несколько флажков:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="16dp">
 
    <TextView android:id="@+id/selection"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="26sp"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"/>
 
    <CheckBox android:id="@+id/java"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Java"
        android:textSize="26sp"
 
        android:onClick="onCheckboxClicked"
 
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/selection"/>
 
    <CheckBox android:id="@+id/kotlin"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Kotlin"
        android:textSize="26sp"
 
        android:onClick="onCheckboxClicked"
 
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/java"/>
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

На каждый флажок можно повесить свой обработчик нажатия. А можно сделать один, как в данном случае. В этом случае мы можем обработать несколько флажков в коде java с помощью конструкции switch...case

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.view.View;
import android.widget.CheckBox;
import android.widget.TextView;
import android.widget.Toast;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
 
    public void onCheckboxClicked(View view) {
        // Получаем флажок
        CheckBox checkBox = (CheckBox) view;
        // Получаем, отмечен ли данный флажок
        boolean checked = checkBox.isChecked();
 
        TextView selection = findViewById(R.id.selection);
 
         // Смотрим, какой именно из флажков отмечен
        switch(view.getId()) {
            case R.id.java:
                if (checked)
                    Toast.makeText(this, "Вы выбрали Java ",Toast.LENGTH_LONG).show();
                break;
            case R.id.kotlin:
                if (checked)
                    Toast.makeText(this, "Вы выбрали Kotlin",Toast.LENGTH_LONG).show();
                break;
            default:
                selection.setText("");
        }
    }
}
```

С помощью конструкции switch...case можно получить id нажатого флажка и выполнить соответствующие действия.

Правда, если нам просто надо взять текст из выбранного флажка, то необязательно в данном случае использовать конструкцию switch, так как мы можем сократить весь код следующим образом:

```java
public void onCheckboxClicked(View view) {
    // Получаем флажок
    CheckBox language = (CheckBox) view;
    // Получаем, отмечен ли данный флажок
    TextView selection = findViewById(R.id.selection);
    if(language.isChecked())
        selection.setText(language.getText());
}
```

Однако в данном случае остается проблема: в текстовом поле отображается только один выделенный элемент. Изменим код MainActivity, чтобы отображать оба выделенных элемента:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.view.View;
import android.widget.CheckBox;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
 
    public void onCheckboxClicked(View view) {
 
        // Получаем флажки
        CheckBox java = findViewById(R.id.java);
        CheckBox kotlin = findViewById(R.id.kotlin);
        String selectedItems = "";
        if(java.isChecked())
            selectedItems +=java.getText() + " ";
        if(kotlin.isChecked())
            selectedItems +=kotlin.getText();
 
        TextView selection = findViewById(R.id.selection);
        selection.setText(selectedItems);
    }
}
```

### OnCheckedChangeListener

Применение слушателя OnCheckedChangeListener представляет альтернативный способ отслеживания изменения флажка. Этот слушатель срабатывает, когда мы устанавливаем или убираем отметку на флажке. Например, определим следующий checkbox:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="16dp">
 
    <TextView android:id="@+id/selection"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="26sp"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"/>
 
    <CheckBox android:id="@+id/enabled"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Включить"
        android:textSize="26sp"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/selection"/>
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

В коде MainActivity подключим обработчик изменения состояния:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.widget.CheckBox;
import android.widget.CompoundButton;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
 
        TextView selection = findViewById(R.id.selection);
        CheckBox enableBox = findViewById(R.id.enabled);
 
        enableBox.setOnCheckedChangeListener(new CompoundButton.OnCheckedChangeListener() {
            public void onCheckedChanged(CompoundButton buttonView, boolean isChecked) {
 
                if(isChecked) {
                    selection.setText("Включено");
                    buttonView.setText("Выключить");
                }
                else {
                    selection.setText("Выключено");
                    buttonView.setText("Включить");
                }
            }
        });
    }
}
```

Слушатель OnCheckedChangeListener определен в базовом классе CompoundButton и определяет один метод - onCheckedChanged. Первый параметр этого метода buttonView - сам измененный флажок CheckBox. А второй параметр isChecked указывает, отмечен ли флажок.

При изменении состояния флажка будет выводиться во всплывающем окне соответствующее уведомление.

## 3.8 Java и Android | ToggleButton

ToggleButton подобно элементу CheckBox может пребывать в двух состояниях: отмеченном и неотмеченном, причем для каждого состояния мы можем отдельно установить свой текст. Например, определим следующий элемент ToggleButton:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="16dp">
 
    <ToggleButton
        android:id="@+id/toggle"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textOn="Включено"
        android:textOff="Выключено"
        android:onClick="onToggleClicked"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Атрибуты android:textOn и android:textOff задают текст кнопки в отмеченном и неотмеченном состоянии соответственно. И также, как и для других кнопок, мы можем обработать нажатие на элемент с помощью события onClick. В этом случае определим в классе Activity обработчик события:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.view.View;
import android.widget.Toast;
import android.widget.ToggleButton;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
    public void onToggleClicked(View view) {
 
        // включена ли кнопка
        boolean on = ((ToggleButton) view).isChecked();
        if (on) {
            // действия если включена
            Toast.makeText(this, "Свет включен", Toast.LENGTH_LONG).show();
        } else {
            // действия, если выключена
            Toast.makeText(this, "Свет выключен!", Toast.LENGTH_LONG).show();
        }
    }
}
```

Создание элемента ToggleButton в коде java:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
import androidx.constraintlayout.widget.ConstraintLayout;
 
import android.os.Bundle;
import android.view.View;
import android.widget.Toast;
import android.widget.ToggleButton;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        //setContentView(R.layout.activity_main);
        ConstraintLayout layout = new ConstraintLayout(this);
        ConstraintLayout.LayoutParams layoutParams = new ConstraintLayout.LayoutParams
                (ConstraintLayout.LayoutParams.WRAP_CONTENT, ConstraintLayout.LayoutParams.WRAP_CONTENT);
        ToggleButton toggleButton = new ToggleButton(this);
        toggleButton.setTextOff("Выключено");
        toggleButton.setTextOn("Включено");
        toggleButton.setText("Выключено");
        toggleButton.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                boolean on = ((ToggleButton) view).isChecked();
 
                if (on) {
                    Toast.makeText(getApplicationContext(), "Свет включен", Toast.LENGTH_LONG).show();
                } else {
                    Toast.makeText(getApplicationContext(), "Свет выключен!", Toast.LENGTH_LONG).show();
                }
            }
        });
        layoutParams.leftToLeft = ConstraintLayout.LayoutParams.PARENT_ID;
        layoutParams.topToTop = ConstraintLayout.LayoutParams.PARENT_ID;
        layout.addView(toggleButton);
        setContentView(layout);
    }
}
```

## 3.9 Java и Android | RadioButton

Схожую с флажками функциональность предоставляют переключатели, которые представлены классом RadioButton. Но в отличие от флажков единовременно в группе переключателей мы можем выбрать только один переключатель.

Чтобы создать список переключателей для выбора, вначале надо создать объект RadioGroup, который будет включать в себя все переключатели:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="16dp">
 
   <TextView android:id="@+id/selection"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="26sp"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"/>
 
    <RadioGroup
        android:id="@+id/radios"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/selection"
        >
 
        <RadioButton android:id="@+id/java"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Java" />
        <RadioButton android:id="@+id/kotlin"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Kotlin" />
    </RadioGroup>
</androidx.constraintlayout.widget.ConstraintLayout>
```

Поскольку класс RadioGroup является производным от LinearLayout, то мы также можем задать вертикальную или горизонтальную ориентацию списка, при том включив в него не только собственно переключатели, но и другие объекты, например, кнопку или TextView.

В классе MainActivity определим обработку выбора переключателей:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.view.View;
import android.widget.RadioButton;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
    TextView selection;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
 
        selection = findViewById(R.id.selection);
        // устанавливаем обработчики для кнопок
        findViewById(R.id.java).setOnClickListener((view)->onRadioButtonClicked(view));
        // устанавливаем обработчики для кнопок
        findViewById(R.id.kotlin).setOnClickListener((view)->onRadioButtonClicked(view));
    }
    public void onRadioButtonClicked(View view) {
        RadioButton radio = (RadioButton) view;
        // если переключатель отмечен
        boolean checked = radio.isChecked();
        // получаем текст нажатой радиокнопки
        String text = radio.getText().toString();
        // Получаем нажатый переключатель
        switch(text) {
            case "Java":
                if (checked) selection.setText("Выбрана Java");
                break;
            case "Kotlin":
                if (checked) selection.setText("Выбран Kotlin");
                break;
        }
    }
}
```

### OnCheckedChangeListener

Кроме обработки нажатия на каждый отдельный переколючатель мы можем в целом повесить на весь RadioGroup с его переключателями слушатель OnCheckedChangeListener и обрабатывать в нем нажатия. Для этого уберем из разметки у элемента RadioGroup определим id:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="16dp">
 
   <TextView android:id="@+id/selection"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="26sp"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent"/>
 
    <RadioGroup
        android:id="@+id/radios"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/selection">
        <RadioButton android:id="@+id/java"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Java" />
        <RadioButton android:id="@+id/kotlin"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Kotlin" />
    </RadioGroup>
</androidx.constraintlayout.widget.ConstraintLayout>
```

Далее в коде MainActivity повесим на объект RadioGroup слушатель OnCheckedChangeListener:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.widget.RadioButton;
import android.widget.RadioGroup;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
    TextView selection;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
 
        selection = findViewById(R.id.selection);
        // получаем объект RadioGroup
        RadioGroup radios = findViewById(R.id.radios);
        // обработка переключения состояния переключателя
        radios.setOnCheckedChangeListener((radiogroup, id)-> {
 
            // получае выбранную кнопку
            RadioButton radio = findViewById(id);
            switch (radio.getText().toString()) {
                case "Java":
                    selection.setText("Выбрана Java");
                    break;
                case "Kotlin":
                    selection.setText("Выбран Kotlin");
                    break;
                default:
                    break;
            }
        });
    }
}
```

Слушатель RadioGroup.OnCheckedChangeListener определяет метод onCheckedChanged(), в который передается объект RadioGroup и id выделенного переключателя. Далее также мы можем получить по id выбранную радиокнопку и выполнить определенную обработку.

## 3.10 Java и Android | DatePicker

DatePicker представляет элемент для выбора даты. Среди его атрибутов можно отметить следующие:

 -   android:calendarTextColor: цвет текста календаря

  -  android:calendarViewShown: указывает, будет ли отображаться вид календаря

  -  android:datePickerMode: устанавливает режим выбора даты

  -  android:dayOfWeekBackground: устанавливает фоновый цвет панели выбора дня недели

  -  android:endYear: устанавливает последний отображаемый год

  -  android:firstDayOfWeek: устанавливает первый день недели

  -  android:headerBackground: устанавливает фоновый цвет для панели выбранной даты

  -  android:maxDate: устанавливает максимальную отображаемую дату в формате mm/dd/yyyy

  -  android:minDate: устанавливает минимальную отображаемую дату в формате mm/dd/yyyy

  -  android:spinnersShown: указывает, будет ли отображаться спиннер в виджете

  -  android:startYear: устанавливает начальный отображаемый год

  -  android:yearListSelectorColor: устанавливает цвет для поля выбора года

Среди методов DatePicker можно отметить следующие:

  -  int getDayOfMonth(): возвращает номер выбранного дня

  -  int getMonth(): возвращает номер выбранного месяца (от 0 до 11)

  -  int getYear()(): возвращает номер выбранного года

  -  void init(int year, int monthOfYear, int dayOfMonth, DatePicker.OnDateChangedListener onDateChangedListener): устанавливает начальную дату. Последний параметр устанавливает слушатель изменения выбранной даты

  -  void setOnDateChangedListener(DatePicker.OnDateChangedListener onDateChangedListener): устанавливает слушатель изменения выбранной даты

  -  void setFirstDayOfWeek(int firstDayOfWeek): устанавливает первый день недели

  -  void updateDate(int year, int month, int dayOfMonth): программно обновляет выбранную дату

Пусть в activity_main.xml определен элемент DatePicker:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="16dp">
 
    <TextView android:id="@+id/dateTextView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="26sp"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
    <DatePicker android:id="@+id/datePicker"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/dateTextView" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Применим некоторые методы DatePicker для управления его поведением:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.widget.DatePicker;
import android.widget.TextView;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
 
        TextView dateTextView = findViewById(R.id.dateTextView);
        DatePicker datePicker = this.findViewById(R.id.datePicker);
 
        // Месяц начиная с нуля. Для отображения добавляем 1.
        datePicker.init(2020, 02, 01, new DatePicker.OnDateChangedListener() {
            @Override
            public void onDateChanged(DatePicker view, int year, int monthOfYear, int dayOfMonth) {
 
                // Отсчет месяцев начинается с нуля. Для отображения добавляем 1.
                dateTextView.setText("Дата: " + view.getDayOfMonth() + "/" +
                        (view.getMonth() + 1) + "/" + view.getYear());
                         
                // альтернативная запись
                // dateTextView.setText("Дата: " + dayOfMonth + "/" + (monthOfYear + 1) + "/" + year);
            }
        });
    }
}
```

Используя метод datePicker.init(); устанавливаем дату по умолчанию - 1 марта 2020 года, так как отсчет месяцев идет с нуля. Кроме того, с помощью последнего параметра - объекта DatePicker.OnDateChangedListener устанавливается обработка выбора даты. Каждый раз, когда пользователь будет выбирать дату, будет срабатывать метод onDateChanged() объекта DatePicker.OnDateChangedListener. Этот метод принимает четыре параметра - view (элемент DatePicker), year (выбранный год), monthOfYear (выбранный месяц), dayOfMonth (выбранный день).

Далее мы можем получить выбранные день, месяц и год. Причем для можно использовать как параметры метода onDateChanged, так и методы самого DatePicker

Начальное состояние перед выбором - установлена дата 1 марта 2020 года.

Выбор произвольной даты (20 мая 2020 года):

DatePicker по умолчанию отображается в режиме календаря, но мы можем использовать добавить другой режим - спиннер с помощью атрибута android:datePickerMode:

```java
<DatePicker android:id="@+id/datePicker"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:datePickerMode="spinner"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/dateTextView" />
```

В данном случае спиннер отображается слева от календаря. Если мы вовсе не хотим отображать календаря, то можно установить атрибут android:calendarViewShown="false"

```java
<DatePicker android:id="@+id/datePicker"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:datePickerMode="spinner"
        android:calendarViewShown="false"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/dateTextView" />
```

## 3.11 Java и Android | TimePicker

TimePicker представляет виджет для выбора времени, который может отображать время либо в 24-часовом, либо в 12-часовом формате.

Среди атрибутов TimePicker следует выделить timePickerMode, который позволяет режим отображения и может принимать одно из двух значений: clock (отображение в виде часов) и spinner (отображение в виде спиннера).

Среди методов TimePicker можно отметить следующие:

    int getHour(): возвращает час (в 24-часом формате)

    int getMinute(): возвращает минуты

    boolean is24HourView(): возвращает true, если используется 24-часовой формат

    void setHour(int hour): устанавливает час для TimePicker

    void setIs24HourView(Boolean is24HourView): устанавливает 24-часовой формат

    void setMinute(int minute): устанавливает минуты

    void setOnTimeChangedListener(TimePicker.OnTimeChangedListener onTimeChangedListener): устанавливает слушатель изменения времени в TimePicker в виде объекта TimePicker.OnTimeChangedListener

Определим TimePicker в activity_main.xml:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="16dp">
 
    <TextView android:id="@+id/timeTextView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="26sp"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
    <TimePicker android:id="@+id/timePicker"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
 
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/timeTextView" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Применим некоторые методы TimePicker для управления его поведением:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.widget.TextView;
import android.widget.TimePicker;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
 
        TextView timeTextView = findViewById(R.id.timeTextView);
        TimePicker timePicker = findViewById(R.id.timePicker);
 
        timePicker.setOnTimeChangedListener(new TimePicker.OnTimeChangedListener() {
            @Override
            public void onTimeChanged(TimePicker view, int hourOfDay, int minute) {
 
                timeTextView.setText("Время: " + hourOfDay + ":" + minute);
                // или так
                // timeTextView.setText("Время: " + view.getHour() + ":" + view.getMinute());
            }
         });
    }
}
```

Для добавления слушателя изменения времени в TimePicker применяется метод setOnTimeChangedListener(), в который передается объект TimePicker.OnTimeChangedListener. Он имеет один метод - onTimeChanged(), который вызывается при каждом изменении времени в TimePicker. Этот метод принимает три параметра - сам элемент TimePicker, hourOfDay - установленный час и minute - установленные минуты. В данном случае просто передаем значение выбранного времени в TextView.

По умолчанию TimePicker отображается в режиме "clock" или часы. Применим режим "spinner":

```java
<TimePicker android:id="@+id/timePicker"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:timePickerMode="spinner"
    app:layout_constraintLeft_toLeftOf="parent"
    app:layout_constraintTop_toBottomOf="@+id/timeTextView" />
```

## 3.12 Java и Android | Ползунок SeekBar

Элемент SeekBar выполняет роль ползунка, то есть шкалу делений, на которой мы можем менять текущую отметку.

Среди его атрибутов можно отметить следующие:

  -  android:max: устанавливает максимальное значение

  -  android:min: устанавливает минимальное значение

  -  android:progress: устанавливает текущее значение, которое находится в диапазоне между минимальным и максимальным

Для управления SeekBar определяет ряд методов, из которых выделим следующие:

-    void setProgress(int progress): устанавливает текущее значение ползунка

-    void setMin(int min): устанавливает минимальное значение

 -   void setMax(int max): устанавливает максимальное значение

-    void incrementProgressBy(int diff): увеличивает текущее значение на diff

-    int getMax(): возвращает максимальное значение

-    int getMin(): возвращает минимальное значение

 -   int getProgress(): возвращает текущее значение

 -   void setOnSeekBarChangeListener(SeekBar.OnSeekBarChangeListener l): устанавливает слушателя изменения значения в SeekBar

Определим SeekBar в разметке layout:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="16dp">
 
    <SeekBar
        android:id="@+id/seekBar"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:progress="20"
        android:max="50"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Атрибут android:progress задает число 20 в качестве текущего значения ползунка, а атрибут android:max - максимально возможное значение - число 50. В итоге мы получим следующий элемент:

Теперь используем метод setOnSeekBarChangeListener(), который позволяет установить обработчики событий изменения значения ползунка. Так, определим в файле layout следующий код:

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:padding="16dp">
 
    <TextView android:id="@+id/seekBarValue"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="26sp"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
 
    <SeekBar
        android:id="@+id/seekBar"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:progress="20"
        android:max="50"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/seekBarValue" />
 
</androidx.constraintlayout.widget.ConstraintLayout>
```

Здесь определен элемент TextView, который будет выводить текущее значение ползунка при его изменении.

И изменим код MainActivity:

```java
package com.example.viewapp;
 
import androidx.appcompat.app.AppCompatActivity;
 
import android.os.Bundle;
import android.widget.SeekBar;
import android.widget.TextView;
import android.widget.TimePicker;
 
public class MainActivity extends AppCompatActivity {
 
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
 
        SeekBar seekBar = findViewById(R.id.seekBar);
        TextView textView = findViewById(R.id.seekBarValue);
        seekBar.setOnSeekBarChangeListener(new SeekBar.OnSeekBarChangeListener() {
            @Override
            public void onProgressChanged(SeekBar seekBar, int progress, boolean fromUser) {
 
                textView.setText(String.valueOf(progress));
            }
 
            @Override
            public void onStartTrackingTouch(SeekBar seekBar) {
 
            }
 
            @Override
            public void onStopTrackingTouch(SeekBar seekBar) {
 
            }
        });
    }
}
```

В метод setOnSeekBarChangeListener() передается объект SeekBar.OnSeekBarChangeListener, который позволяет установить три метода-обработчика:

-    onProgressChanged: срабатывает при перетаскивании ползунка по шкале. Передаваемый в метод параметр progress позволяет получить новое значение ползунка, которое в данном случае передается в TextView для отображения на экране

-    onStartTrackingTouch: срабатывает при начале перетаскивания ползунка по шкале

-    onStopTrackingTouch: срабатывает при завершении перетаскивания ползунка по шкале

Также мы можем получить текущее значение ползунка, использовав метод getProgress():

```java
public void onProgressChanged(SeekBar seekBar, int progress, boolean fromUser) {
 
    textView.setText(String.valueOf(seekBar.getProgress()));
}
```
