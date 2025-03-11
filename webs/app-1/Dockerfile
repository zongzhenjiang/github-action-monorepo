# 使用合适的基础镜像，假设你使用的是 Nginx 来部署构建的静态文件
FROM nginx:alpine

# 复制 dist 文件夹中的内容到 Nginx 的默认静态文件目录
COPY dist/ /usr/share/nginx/html/

# 如果你有其他配置文件，比如自定义的 nginx 配置文件，你可以添加它
# COPY nginx.conf /etc/nginx/nginx.conf

# 暴露 80 端口
EXPOSE 80

# 启动 Nginx
CMD ["nginx", "-g", "daemon off;"]