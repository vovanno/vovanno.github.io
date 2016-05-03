---
layout: post
title: Shopify, ты кто такой?
---

#### Краткий обзор самой популярной CMS для E-Commerce.

<image src='../images/hello-shopify.jpg' />

```Вода mode: on```

В наше время аббревиатурой [**CMS**](https://ru.wikipedia.org/wiki/%D0%A1%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%B0_%D1%83%D0%BF%D1%80%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D1%8F_%D1%81%D0%BE%D0%B4%D0%B5%D1%80%D0%B6%D0%B8%D0%BC%D1%8B%D0%BC) не испугаешь даже школьника. Некоторые из них, выпускаясь из школы могут легко написать вам сайт визитку или простенькую "интернет витрину" используя **Joomla** или **WordPress**. Но рано или поздно рынку было недостаточно простых сайтов, содержащих контент о человеке или организации. И все бы ничего: нужен сложный функционал - плати кучу денег бездельникам-программистам и они тебе напишут то, что ты хочешь или, по крайней мере, что-то похожее.

Поэтому рано или поздно возник вопрос: а не написать ли нам что-то вроде ```Joomla```, но чтобы можно было создать интернет магазин? Как следствие, на сегодняшний день у нас есть десятки различных ```CMS```, написанных под различные платформы, реализующих приблизительно один и тот же функционал, в лучшем случае, имеющих разные подходы к реализации **E-Commerce** систем.

Ruby on Rails не исключение, поэтому я решил исследовать и рассказать о них немного больше, чем просто "[любое_имя_cms] - это штука для интернет магазина". Чтобы не перегружать статью материалом, я решил написать по отдельной статье про три самых популярных E-Commerce системы

* Shopify
* Spree
* Shoppe

Остальные существующие, на мой взгляд, либо слишком сырые, либо форки от Spree.

Цель моих статей - собрать описание этих CMS в одном месте, на русском языке, чтобы можно было делиться информацией с другими людьми, да и просто изложить мои мысли письменно, на память, так сказать :)

```Вода mode: off```

## Что такое Shopify

Для начала почему я пишу про [**Shopify**](https://www.shopify.com/), как **CMS** под [**Ruby on Rails**](http://rubyonrails.org/). На самом деле, все что связывает Shopify и Ruby on Rails, так это то, что Shopify был написан с использованием этого фреймворка. Все. Однако, несмотря на это, Shopify остается на слуху на рынке разработки под Ruby on Rails, где, на мой взгляд, часть заказчиков и исполнителей считают что для того, чтобы создать интернет магазин на Shopify необходимо участие RoR разработчика. Однако это не так...

По большому счету, **Shopify** - платформа с закрытым исходным кодом для ведения торгового бизнеса через сеть интернет, предоставляющая возможность:

* управлять товарами: создание товаров, условия доставки, коллекции товаров, подарочные сертификаты.
* управлять заказами.
* управлять списками пользователей: просмотр делатей по каждому пользователю, фильтры, списки для рассылки.
* отчеты: более 10 видов отчетов по деятельности нашего предприятия.
* карты скидок.
* управление интернет-магазином(подробнее дальше)

При всем при этом, в нашем распоряжении есть еще уйма настроек и прочих полезностей. Несмотря на английский язык, у Shopify достаточно понятный интерфейс, поэтому описывать что как можно сделать я не буду. Тем более это не цель данной статьи. Дальше я буду рассматривать только интернет магазин Shopify.

Для начала работы с Shopify необходимо зарегистрировать аккаунт. Тут же есть возможность создать пробный аккаунт. Для пробного аккаунта будут доступны все функции Shopify, но интернет магазин не будет доступен в сети интернет.
После регистрации аккаунта Shopify нам будет доступна ```Dashboard``` - раздел управления нашим аккаунтом. Отсюда мы имеем доступ ко всем функциям системы.

## Shopify Online Store

Создание интернет магазина занимает от силы 30 секунд. Для создания магазина достаточно перейти на главную страницу Dashboard и нажать кнопку создания интернет магазина и выбрать тему.

К слову о темах. Изначально у нас есть на выбор несколько бесплатных и много платных тем на любой вкус. Если мы не нашли ничего подходящего - можно создать тему самому. Создание темы - отдельный разговор и рассматривать здесь я его не буду. Единственное, что могу сказать - для создания темы достаточно будет верстальщика, который уделит 5 минут на изучение [Liquid](http://liquidmarkup.org/).

В дополнение к магазину, который имеет полный стек функций, необходимых для традиционного магазина в интернете, включая [платежную систему Shopify](https://docs.shopify.com/manual/payment-settings/shopify-payments), нам любезно предоставляют возможность вести ```блог```, который можно присоединить к сайту.

Помимо стандартных страниц вроде заглавной, страниц продуктов и других типичных страниц для магазина у нас есть возможность создавать произвольные статические страницы вроде `Terms & conditions` или ```About```. Ссылки на эти страницы нужно будет самим прописать в шаблон магазина.

Дополнительно, мы можем сами настраивать навигацию нашего магазина и управлять доменами.

## Кастомизация

Shopify кастомизируется только в рамках описанного мной выше. Мы не можем добавлять дополнительные поля для товаров или заказов, не можем их переименовывать(только на уровне шаблона).

## Shopify Apps

Для расширения фунационала системы, как и в других популярных CMS, в Shopify присутствуют плагины. Внутри системы они называются Apps. Мы можем установить любое приложение из списка доступных, или же создать свое. Приложение, которое мы пишем самостоятельно(коорого нет в магазине приложений), называется **Embedded App**. Embedded App может быть разработано на любом языке под любой платформой. Единственное требование - это должно быть веб-приложение. Для встраивания Embedded App используется ```Iframe```, в котором будет отображаться наше приложение. Embedded App общается с Shopify посредством ```Shopify API```.

Да, мы можем разработать приложения для Shopify используя Ruby on Rails. Этот факт дополнительно вводит нас в заблуждение, что Shopify - это что-то под RoR. Несмотря на это, Embedded App может быть разработан, например, с использованием PHP.

## Что мы можем сделать как программисты, кроме Ebeded App?

Максимум, что мы можем сделать как программисты - это использовать Shopify API для наших нужд, но, честно говоря, я не увидел практического применения Shopify API в обход Shopify - деньги нам все равно платить придется, а магазин проще и быстрее создать средставами самого Shopify.

## Выводы

Еще раз повторюсь, что это обзорная статья и деталей работы с системой я не раскрывал специально.

Мое мнение: **Shopify** - полноценная, самостоятельная и мощная **E-Commerce система**, которая покрывает полный стек бизнес-процессов, необходимых для ведения бизнеса в интернет, связанного с продажей товаров. В принципе, мы можем продавать и услуги, но, обычно, для этого достаточно более простых решений. Несмотря на цену, а Shopify, как и следовало ожидать, платная система - **29 долларов в месяц и 2% от продаж** за базовую версю вполне справедливая цена, если учитывать весь функционал, который мы получим.

Для управления системой достаточно иметь голову на плечах и максимум верстальщика для редактирования шаблона под ваши нужны. Может быть это кому-то покажется грустным - но разработчики Ruby on Rails нужны максимум для разработки плагина для Shopify и не более того. С тем же успехом, этот плагин может быть написан и на другом языке.

P.S. Слово ```Shopify``` встречается в тексте статьи 30 раз...

<!--There is disqus comments code below-->

<div id="disqus_thread"></div>
<script>

var disqus_config = function () {
this.page.url = 'http://murzvo.github.io/Hello-Shopify/';
this.page.identifier = 'murzvo.github.io/Hello-Shopify';
};

(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');

s.src = '//muzakvladimir.disqus.com/embed.js';

s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript" rel="nofollow">comments powered by Disqus.</a></noscript>