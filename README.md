# docker-khmer
Docker ជា  platform ប្រើដើម្បី developing, shipping, and running applications. Docker ត្រូវបានប្រើដំបូងក្នុងខែ មីន ឆ្នាំ ២០១៣.
![docker-tutorial](https://user-images.githubusercontent.com/74696117/226498072-7ede4468-ca13-4e51-86a7-34f2b57b8c7f.png)
## Docker ជាអ្វី?
## CLI

| Command line                                              | Description                                   |
| :-------------------------------------------------------- | :---------------------------------------------|
| `docker image`                                            | ប្រើដើម្បីមើលថាតើ Docker របស់យើងមាន Image អីខ្លះ |
| `docker run -it ubuntu /bin/bash`                         | ប្រើដើម្បី Install Ubuntu ក្នុង Docker របស់យើងលះ  |
| `apt install net-tools`                                   | ប្រើដើម្បី install tool confin (ក្នុង Ubuntu)      |
| `docker ps -a`                                            |  ប្រើដើម្បីមើល container ទាំងអស់.                |
| `docker container start (ID របស់ Contaiter) /bin/bash`    | Run container តាមរយៈ ID                       |
| `docker container stop (ID របស់ Contaiter)`               | Stop container តាមរយៈ ID                      |
| `docker excec -it (ID របស់ Contaiter)`                    | ចូលទៅកាន់ Container តាមរយៈ ID                |
| `docker container rm  (ID របស់ Contaiter)`                | Delete container តាមរយៈ ID                    |
