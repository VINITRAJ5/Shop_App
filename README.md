# Screenshot of This App Below <h1>

## This is the HomePage of App <h2>
   
<img src="https://github.com/VINITRAJ5/Shop_App/blob/master/Screenshots/1%20(1).jpg" width="280">

 1. it have favourite icon to choose your Favourite
   1. and has cart button where you can add product to your cart
   
  ## This is the Cart Section of App <h2> 
<img src="https://github.com/VINITRAJ5/Shop_App/blob/master/Screenshots/1%20(2).jpg" width="280">

This Screen Contain Information of Following

> 1.Total Purchase Item
>> 2.Quantity of every Product or you can say Count
>>> 3.Total Amount Calculated
   
   
<img src="https://github.com/VINITRAJ5/Shop_App/blob/master/Screenshots/1%20(3).jpg" width="280">
   
  *More Preview of App* 

<img src="https://github.com/VINITRAJ5/Shop_App/blob/master/Screenshots/1%20(4).jpg" width="280">

   ## This is the Product Addition Form of App <h2>
   **You can Add New Products Here**
   
<img src="https://github.com/VINITRAJ5/Shop_App/blob/master/Screenshots/1%20(5).jpg" width="280">

   ### This is the Product Detail Page of App <h3>
<img src="https://github.com/VINITRAJ5/Shop_App/blob/master/Screenshots/1%20(6).jpg" width="280">

  
  
 For Installation of this App 
   Clone The code and
   then Run first this command in your editor terminal `flutter pub get` then  `flutter run`
   
### Snippets Of `main.dart`
 
  ```
   class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MultiProvider(
      providers: [
        ChangeNotifierProvider.value(
          value: Products(),
        ),
        ChangeNotifierProvider.value(
          value: Cart(),
        ),
        ChangeNotifierProvider.value(
          value: Orders(),
        ),
      ],
      child: MaterialApp(
          title: 'MyShop',
          theme: ThemeData(
            primarySwatch: Colors.purple,
            accentColor: Colors.deepOrange,
            fontFamily: 'Lato',
          ),
          home: ProductsOverviewScreen(),
          routes: {
            ProductDetailScreen.routeName: (ctx) => ProductDetailScreen(),
            CartScreen.routeName: (ctx) => CartScreen(),
            OrdersScreen.routeName: (ctx) => OrdersScreen(),
            UserProductsScreen.routeName: (ctx) => UserProductsScreen(),
            EditProductScreen.routeName: (ctx) => EditProductScreen(),
          }),
    );
  }
}
```
  
  IF you get issue or error  create a issue i'll Love to help
