FVANG
=======

### Flask-Vagrant-Ansible-Nginx-Gunicorn *Starter Pack*

##### Getting started

0. Install [Vagrant](https://www.vagrantup.com/)

0. Clone this repo as your project name:
    ```
    git clone git@github.com:paste/fvang.git NEW-PROJECT-NAME
    ```

0. Configure project name and host name in `ansible/roles/common/vars/main.yml`:
    ```
    project_name: "fvang"
    host_name: "fvang.local"
    ```

0. Modify your local `/etc/hosts`:

    ```
    192.168.33.11   fvang.local
    ```

0. Build your Vagrant VM:

    ```sh
    vagrant up
    ```

0. Log into the VM via SSH:
    ```sh
    vagrant ssh
    ```

0. Start Flask development server:
    ```sh
    cd ~/fvang
    python app/app.py
    ```

0. Profit :heavy_check_mark:
