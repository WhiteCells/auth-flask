### Flask 后台权限管理系统

基于Python的Flask WEB框架实现后台权限管理系统
内容包含：用户管理、角色管理、资源管理和机构管理。

### 后端

**后端依赖插件**

 1. Flask
 2. Flask-SQLAlchemy
 3. Flask-Login
 4. Flask-moment
 5. MySQL-connector-python
 6. Flask-Excel

```sh
pip3 install -r requirements.txt
```

更改config.py DevelopmentConfig类下的数据库连接，提供用户名密码。

```sh
python3.x -m flask --app start run [-h 0.0.0.0] [-p 8080]

python -m flask --app start run -h 0.0.0.0 -p 8080
```

### 前端

**前端依赖插件**

 1. Vue
 2. Vuex
 3. ElementUI
 4. Axios

1. 安装Node.js 16
2. 进入源代码的ui目录。cd ui
3. npm install
4. npm run dev

- 首页
- 个人中心
- 机构管理
- 角色管理
- 用户管理
- 资源管理
- 登录历史

系统默认的登录名密码为admin/123456