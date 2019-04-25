How to build:

```bash
git clone https://github.com/journeymidnight/librbd-test.git
cd librbd-test
sudo apt install build-essential cmake librbd1 librados2
cmake CMakeLists.txt
make
```

How to run:

```bash
./rbd_example -c ceph_config_example.conf
```