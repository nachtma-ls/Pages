# Pages en Xamarin
Los Pages son elementos visuales que ocupan toda o la mayor parte de la pantalla, funcionan como los contenedores principales para organizar nuestros elementos secundarios.

![image](https://user-images.githubusercontent.com/84193239/236698976-c55ce826-235a-4f29-ab35-003b027a5a67.png)

## ContentPage
* Es el page mas simple y común
* Normalmente tiene objetos de vista que suelen ser diseñados con StackLayout, Grid o ScrollView

![image](https://user-images.githubusercontent.com/84193239/236699056-21d66847-83b8-40e7-9afe-abf26838f971.png)

## NavigationPage
* Es el administrador de la navegación entre otras páginas mediante el uso de pilas con funciones pop y push respectivamente
* Nos permite aplicar varias ventanas a nuestra app

![image](https://user-images.githubusercontent.com/84193239/236699175-6ef365b0-7ec5-4614-8730-45cc5de038b2.png)

## FlyoutPage
* Administra 2 paneles de información por medio de una lista o un menú
* Muy utilizado a la hora de querer aplicar una barra desplazable

![image](https://user-images.githubusercontent.com/84193239/236699252-bd4c5fc7-8fde-4393-bfbe-2e5cdca2c51d.png)

## TabbedPage
* Permite la navegación entre páginas secundarias usando pestañas
* Algunos ejemplos que usan este tipo de navegación son WhatsApp y Messenger

![image](https://user-images.githubusercontent.com/84193239/236699314-8759fe50-33dd-42c1-b581-8d9ac0db3f8b.png)

## CarouselPage
* Permite navegar entre páginas secundarias deslizando el dedo hacia la izquierda o derecha.
* Muy comodo visualmente

![image](https://user-images.githubusercontent.com/84193239/236699367-1a1c6d85-52f2-4814-b995-5537c761f5f7.png)

## Uso
A contiuación se dejan los ejemplos de cada page mencionado anteriormente:
> Es necesario modificar en el App.xaml.cs la ventana principal para ver cada uno de los ejemplos.
```
using System;
using Xamarin.Forms;
using Xamarin.Forms.Xaml;

namespace Pages1
{
    public partial class App : Application
    {
        public App()
        {
            InitializeComponent();

            //MainPage = new NavigationPage(new Page1());
            //MainPage = new FlyoutPage1();
            MainPage = new TabbedPage1();
        }

        protected override void OnStart()
        {
        }

        protected override void OnSleep()
        {
        }

        protected override void OnResume()
        {
        }
    }
}
```
