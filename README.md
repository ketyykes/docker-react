
在這個 branch 的終端機介面輸入以下指令

```
docker build -t my-react:dev .

# 使用 Dockerfile 在當前目錄(.)構建一個名為 'my-react:dev' 的 Docker 映像
# '-t' 選項用於為映像指定一個標籤名稱
```

```
docker run --name my-react-container3000 -d -p 3000:5173 my-react:dev

# 使用 'docker run' 命令來運行名為 'my-react:dev' 的映像
# '--name' 給創建的容器指定一個名稱 'my-react-container3000'
# '-d' 選項讓容器在後臺運行
# '-p 3000:5173' 表示將主機的 3000 端口映射到容器的 5173 端口
```