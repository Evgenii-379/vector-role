Role vector-role
=========

Эта роль устанавливает и настраивает Vector на целевых хостах.

Requirements
------------

- ​​Ansible 2.10.8


- Целевой хост должен иметь доступ к локальному файлу .deb для установки Vector.

Role Variables
--------------

Для этой роли можно задать следующие переменные:

- `vector_version`: 
- По умолчанию: `"0.43.0"`
- Описание: Версия Vector для установки.

- `local_vector_file`: 
- По умолчанию: `"/home/evgenii/Загрузки/vector_0.43.0-1_amd64.deb"`
- Описание: Путь к локальному файлу .deb для установки Vector.

Dependencies
------------

Эта роль не имеет зависимостей от других ролей.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

- hosts: vector
  become: true
  roles:
    - vector-role


License
-------

BSD

Author Information
------------------

Эта роль была создана в 2024 году [Evgenii](mailto:your.email@example.com).
