# NGS
# 部署

创建虚拟环境
cd backend
uv sync

初始化数据库
# Let the DB start
python app/backend_pre_start.py

# Run migrations
alembic upgrade head

# Create initial data in DB
python app/initial_data.py


前端
npm run generate-client
npm install

npm run dev

拉取最新代码
git pull origin master