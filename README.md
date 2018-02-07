# Yelp Maps
Visualization of restaurant ratings using machine learning and the Yelp academic dataset made for CS61A at UC Berkeley.

Predicting your own ratings:  
1. In the users directory, you'll see a couple of .dat files. Copy one of them and rename the new file to yourname.dat (for example, tina.dat).
2. In the new file (e.g. tina.dat), you'll see something like the following:
```
make_user(
    'Tina Nguyen',     # name
    [                   # reviews
        make_review('Jasmine Thai', 4.0),
        ...
    ]
```
Replace the second line with your name (as a string).  

3. Replace the existing reviews with reviews of your own! You can get a list of Berkeley restaurants with the following command:  
```
python3 recommend.py -r
```
Rate a couple of your favorite (or least favorite) restaurants.  

4. Use recommend.py to predict ratings for you:  
```
python3 recommend.py -u tina -k 2 -p -q Sandwiches
```
(Replace tina with your name.)   

You can play around with the number of clusters (the -k option) and try different queries (with the -q option)
