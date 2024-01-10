# First thing you need to have docker desktop

# Only for MacOS
Download this file from link: https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-2/wkhtmltox_0.12.6.1-2.bullseye_arm64.deb and replace file in folder packages

# Build image hr:16
cd box
sudo docker build -t hr:16 {path-to-box-folder} 
  Example: sudo docker build -t hr:16 /home/sunny/BK-Tennis-CLB/box

# Clone odoo repository
cd..
git clone -b 16.0 --single-branch https://github.com/odoo/odoo.git

# Run Docker Compose
sudo docker-compose up -d