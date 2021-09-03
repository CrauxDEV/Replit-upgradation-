# Replit-upgradation
Here is a solution for updating node version in [Replit.com](https://replit.com/~)

# Introduction 
Recently discord.js have released `discord.js@v16`, which needs node version `node@16`!
If you create a node.js project in replit you will see the version will be `nodev12`.
So in case of updating node version, [Replit.com](https://replit.com/~)will update node version automatically but it will take some time.
Now let's talk about how can we do the same thing by manually?

# Trick/Solution 
1st step :- Create a new project with language `nix(beta)` instead `node.js`
<br />
2nd step :- You have to replace the following code with the old one in `.replit` file
```.replit
run = "node index.js"
```
<br />
3rd step :- Now open `replit.nix` file and there replace the following code with old one

```
{ pkgs }: {
	deps = [
    pkgs.nodejs-16_x
	];

}
```
Now , Our project has been upgraded to Nodev16

# Check
For checking open shell or console, there type `node -v`.
If it shows `nodev16` then our project is ready !

# Cautions
Remember in this project all the packages will not be installed automatically by replit, you have to do manually using shell or console!else codes will not run properly!

# Support
If any help about this solutions then contact me ;
[Instagram](https://instagram.com/ig_crauxop)
<br />
[Discord Server](https://discord.ink/galaxystudio)
