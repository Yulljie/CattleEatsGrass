# 得本文于本地之法

## 法一：克隆本站

    git clone https://github.com/Yulljie/CattleEatsGrass.git

## 法二：构建

<i>（有误，等待修正）</i>

1. 安装python    
    - Arch linux：  

            pacman -Sy python

    - Debian：  

            apt install python

2. 安装material for mkdocs  

        pip install mkdocs-material

4. 使用mkdocs创建新文档  

        mkdocs new

5. 移除文件docs/index.md  

        rm docs/index.md

6. 克隆原markdown文档仓库到docs文件夹  

        cd docs
        git clone https://github.com/Yulljie/test.git

7. 回到上层目录并创建目标文件夹  

        cd ..
        mkdir target

8. 构建文档

        mkdocs build -t material -d target

