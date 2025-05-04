##  Pacman Guide
this guide inspired by (https://wiki.archlinux.org/title/Pacman).

* synchronizes the repository databases and updates the local packages

  ```bash
  pacman -Syu
  ```
  
* search for packages in the repository database
  
  ```bash
  pacman -Ss [package-name]
  ```

* get detail information about package 
  
  ```bash
  pacman -Si [package-name]
  ```

* list orphan package dependency
  
  ```bash
  pacman -Qdt
  ```

* list upgradable package
  
  ```bash
  pacman -Qu
  ```

* remove package and package that will be orpahn and depends on it
  
  ```bash
  pacman -Rsu [package-name]
  ```

* remove orphan package 
  
  ```bash
  pacman -Rsun $(pacman -Qdtq)
  ```
