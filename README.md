# docker-khmer
Docker ជា  platform ប្រើដើម្បី developing, shipping, and running applications. Docker ត្រូវបានប្រើដំបូងក្នុងខែ មីន ឆ្នាំ ២០១៣.
![docker-tutorial](https://user-images.githubusercontent.com/74696117/226498072-7ede4468-ca13-4e51-86a7-34f2b57b8c7f.png)
## Docker ជាអ្វី?
Docker គឺជា open source platform សម្រាប់ build, deploy និងគ្រប់គ្រង containerized application។
វាអាចជួយឱ្យ developer ផ្តោតទៅលើការសរសេរកូដ និង អភិវឌ្ឍ ជាងការមានកង្វល់ទៅលើ system ឬ OS ណាមួយដែល application នោះនឹងដំណើរការទៅលើ។
## អត្ថប្រយោជន៍សំខាន់ៗដែល Docker ផ្តល់ឱ្យ Developers 
- *** Docker for Everyone:*** វាមានភាពងាយស្រួលក្នុងការចាប់ផ្តើម សូម្បីតែ non-tech ក៏អាចចាប់ផ្តើមបានដែរ ជាមួយនឹង commands ខ្លីៗស្រួលយល់។
- *** Environment Isolation:*** ក្នុងការ​ configure environments សម្រាប់ verison software ផ្សេងៗគ្នានៅលើ machine តែមួយពិតជាពិបាកណាស់។ តែពេលនេះ ជាមួយនឹង docker containers គឺ environments ទាំងនោះនឹងនៅដាច់ៗពីគ្នា​ ធ្វើឱ្យមានភាពងាយស្រួលមិន conflict គ្នាទៅវិញទៅមកទេ។
- *** OS Independent Apps:*** ជាមួយនឹង docker container យើងអាចដាក់ applications របស់យើងឱ្យប្រើប្រាស់បាននៅលើ OS ដូចជា Linux,​ macOS, Windows or ARM-based platforms។
- *** Rapid Development & Development:*** Docker ជួយកាត់បន្ថយពេលវេលាឱ្យយើងបានច្រើនបើសិនជាយើមានការងារដែលធ្វើជា repetitive tasks។ Docker គឺត្រូវបានគេប្រើប្រាស់ច្រើនជាមួយនឹង Continuous Integrations និង Continuous Delivery (CI/CD) workflows ផងដែរ។
- *** Scalability & Flexibility Made Easier:*** Containers ដែលយើងធ្វើការ configure រួចហើយគឺត្រូវបានវេចខ្ចប់នៅក្នុងនោះ ហើយវានឹងផ្តល់ភាពងាយស្រួលក្នុងការ scale និងមានភាព flexible ផងដែរ។ បើសិនជាមានការផ្លាស់ប្តូរ configurations យើងគ្រាន់តែដូរនៅក្នុង docker images តែប៉ុណ្ណោះ។ 
- *** No More Security Issues:*** Docker containers មានសុវត្ថិភាពជាង app ធម្មតា ដោយសារតែ containers មិនអាចធ្វើការ access ទិន្នន័យ នៃ containers ផ្សេងបានទេជា defaults លុះត្រាតែមានការផ្តល់សិទ្ធិ។ ហើយលើសពីនេះ យើងក៏អាចធ្វើការ បន្ថែមនូវ security layers ពីលើនេះបានផងដែរ។
- *** Ship Anytime, Anywhere:*** ការ Migrate និង Shipment App មិនមែន ជាភាពងាយស្រួលដែលត្រូវការតែ human resource នោះទេគឺថែមទាំងតម្រូវឱ្យមានវិជ្ជាជីវ:ខ្ពស់ ក្នុងការ configure និង setup ផងដែរ។ Docker គឺជាអ្នកសម្រាលបន្ទុកទាំងនេះ ដោយយើងអាចធ្វើការ ship app គ្រប់ទីកន្លែងនិងគ្រប់ពេលវេលា។ 
អ្វីដែលយើងត្រូវការគឺ តំឡើង docker នៅលើ target machine និង run commands ដើម្បីឱ្យ project run នៅក្នុងរយ:ពេលដ៏ខ្លី។
- *** Dependency Management Made Easier:*** បើយើងមិនប្រើប្រាស់ docker យើងត្រូវ តំឡើងរាល់ libraries, configs និង services ដូចជា database ឬ cache នៅពេលយើងចង់តំឡើង application លើ server ផ្សេងឬ ទីតាំងផ្សេង។ ជាមួយនឹង Docker ដោយសារតែ វាមាន dependencies management 
នោះគ្រប់ app ឬ project អាច isolate dependencies ទាំងនោះទៅតាមរាល់ container និងអាចដំណើរការ app ដដែលនោះបានច្រើននៅលើ machine តែមួយ។
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
