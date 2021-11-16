## Create React App

To create a react application we can use a frontent tool named **Vite**. This was prefered over create-react-app because its much faster and lighter.

To initialize the react app we can use the following command

```
npm init vite
```

![enter image description here](https://i.imgur.com/OMafTDc.png)

To change the content of the app to _Hello World_ we have to edit the App.jsx file in the source directory and in the return change the content to `Hello World`

![enter image description here](https://i.imgur.com/NZcrUZe.png)

To run the application we can navigate to the react directory and use the following command

```
npm run dev
```

The above command runs the react application on the port 3000

![enter image description here](https://i.imgur.com/T13wHrf.png)

To change the port we can edit the **package.json** file. On the dev section lets change `vite` to `vite --port 3001`.

![enter image description here](https://i.imgur.com/TGnTLMQ.png)

Now again run the command `npm run dev` and we can verify that the react app is now running on the port **3001**

![enter image description here](https://i.imgur.com/cyYUMQy.png)
