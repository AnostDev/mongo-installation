# How to install MongoDB on linux ?


1. Download mongodb [here](https://github.com/AnostDev/mongo-installation).
2. Uncompress the tar in the folder of choice. Here I choosed ~/mongo.

```sh
mkdir -p ~/mongo
tar -xf /path/to/mongo/mongodb-linux-x86_64-ubuntu1604-3.2.22.tgz -C ~/mongo
```

3. Prepare bash/shell for mongo autocompletion

```sh
echo "MONGO_HOME=/usr/bin/mongo" >> ~/.bashrc
```
```sh
echo "export PATH=\$PATH:\$MONGO_HOME/bin >> ~/.bashrc
```

4. Create a symbolink link to mongo
```
sudo ln -s ~/mongo/mongodb-linux-x86_64-ubuntu1604-3.2.22 /usr/bin/mongo
```

5. Update the ~/.bashrc file
```sh
source ~/.bashrc
```