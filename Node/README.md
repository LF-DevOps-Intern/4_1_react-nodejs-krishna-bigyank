We can install Node.js LTS (v16.x) with the help of the following command

```
curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
sudo apt-get install -y nodejs
```

![enter image description here](https://i.imgur.com/81eHlCt.png)

Now lets write two simple web server which runs on port 6080 and 7080.

![enter image description here](https://i.imgur.com/ERox3Yb.png)
To run these web servers we can simply put the following command

```
node server1.js
node server2.js
```

![enter image description here](https://i.imgur.com/iSeLvHZ.png)
The from the above picture we can see that both the web servers are running on the port 6080 and 7080

### Installing PM2

With NPM we can install pm2 on our system:

```
npm install pm2 -g
```

![enter image description here](https://i.imgur.com/8N3Qlpw.png)
To create 4 clusters we can put the following command

```
pm2 start server1.js -i 4
pm2 start server2.js -i 4
```

![enter image description here](https://i.imgur.com/LLmWhm2.png)
To delete the clusters one-by-one we can use the **id** of the each cluster.

```
pm2 delete 0
pm2 delete 1
pm2 delete 2
pm2 delete 3
```

To delete all the clusters we can refer by its name

```
pm2 delete server2
```

The above command deletes all the clusters of the server2

![enter image description here](https://i.imgur.com/GrYzzKq.png)
