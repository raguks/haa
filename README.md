# haa 2019 convention registration and communication portal
This gh-pages hosts family based registration support using paypal customized bootstrap workflow and a website that can be used for community conventions.

<img width="990" alt="screen shot 2019-01-07 at 12 27 12 pm" src="https://user-images.githubusercontent.com/680244/50786058-6e784380-1280-11e9-902e-4a18b5760ede.png">

The html mostly developed using Mobirise tool.

## Setup
1. 
  * Install Mobirise tool(https://mobirise.com/) and then
  * Install git client (and sourceTree if you dont link cmd line or on windows) on your laptop 

2. Fork this git repo and name it say ```haa-fork``` then clone it to your laptop 
```git clone -b gh-pages https://github.com/raguks/haa-fork.git```

3. Import the haa-fork folder you downloaded/cloned from github to Mobirise.

## Updating the portal
4. sponsor.html and register.html will not import correctly - so keep a copy of it elsewhere
```
cp sponsor.html register.html ../backup/.
```

5. Use Mobirise to make changes to index.html as required.
6. Publish the changes to your git repo 
7. Overwrite or merge (if you changed) sponsor.html and register.html from your backup and 

```
cp -rf ../backup/register.html .
cp -rf ../backup/sponsor.html  .
git add sponsor.html register.html 
git commit -m "Over writing working copy of sponsor and register"
git push origin gh-pages
```

Once you confirm the portal is working you can copy to production server.

Contact Ragu Kattinakere if you have questions.
