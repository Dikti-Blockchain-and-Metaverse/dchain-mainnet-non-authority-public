# Info Dchain POA

## RPC : https://mainnet.dchain.id

## Chain Id : 17845

## Monitoring : https://monitoring.dchain.id/

# Daftar Node

## Node UGM

- Authority : Yes
- Running : Yes
- enode : enode://961ddf94040314bf6c3cb877c3724ab5d6bb83a159ce7bc3364c20723e26951514403d7b56c4deaf10a142cf91efab7d0e81c4bac2d2842f111d56909048d44c@node-ugm.dchain.id:30305

## Node UB

- Authority : Yes
- Running : Yes
- enode : enode://fc32005fc49d4940701a4ce77bdc06cc2d1c47da30a71ea5cd2789ac055418a7fbf6751a6c4d0f7460cb01431ed37cacefab99786fbced026958d43412db3759@node-ub.dchain.id:30305

## Node ITS

- Authority : No
- Running : No
- Permasalahan : Tidak bisa terhubung ke server

## Node UT

- Authority : Yes
- Running : Yes
- enode : enode://82179cf70a8cec6096867a86edbddd79aac7cb651586ff123ad58f2cb26fdaa67784e903c8e9a0ae9ea4a483cb81d19bf5227b43e8e3438b154d4ed27880fefc@node-ut.dchain.id:30305

## Node ITB

- Authority : Yes
- Running : Yes
- enode : enode://837a6a464a1e3d050977dd8ce823e18b6ad8f21dc9dda60bd14825c5253a792bd45feb5b77f95a9f31a67dc93662e57f2706699bf31551304452c439ae43d3a5@node-itb.dchain.id:30305

## Node UG

- Authority : Yes
- Running : Yes
- enode : enode://c6c285fb533ebf98612665fd9470621d1c53a450964880815128a24abcf25fddd3252bdd68f0c39dd8a17e0191d37bdd4bc0685a295b83b0781436e12ae272be@node-ug.dchain.id:30305

## Node UNHAS

- Authority : Yes
- Running : Yes
- enode : enode://e560a2a44406a2338e943c4fd6d0ca9d3048719f2dda4a7c33e5c15e9479ad297c5561207616dc3c908f9a76dad342755cc2cd0d4454c0741e512ff353b48142@node-unhas.dchain.id:30305

## Node UMS

- Authority : Yes
- Running : Yes
- enode : enode://99b6e8739260ec92531817995935323c8337a91174e46188743fef64cf1e3eebb84f604dd5c7c1db1a5a0800ffded2f51e8693b16398d0caf6c952d0b31b7bf9@node-ums.dchain.id:30305

## Node DIKTI

- Authority : No
- Running :
- enode : enode://a5f70d62664be2438dfce7133890086e4caa5f9b78e578f3b38faa8ccd0e93444c2e2e141985c048a18aaaf3bd52c131ddbb8ee4f633f27943ecfc67e551d59a@139.255.5.197:59347

# Required Tools

1. Docker v24.0
2. Docker compose v3.7
3. Geth v1.13.2

# Instaling Node

1. Pastikan server sudah terinstall tools yang dibutuhkan.
2. Clone repository ini pada server.
3. Buat file .env dan sesuaikan variabel yg ada.
   Contoh (contoh ini ada juga di file .env.example):

   ```
   NETWORK_ID=17845

   ETH_STATS= <Nama node>:Dchain-POA@monitoring.dchain.id:443         #NodeName:password@linkToEthStats

   PATH_DCHAIN=<path bind folder pada vm>

   BOOTNODE_ENODE= enode://c6c285fb533ebf98612665fd9470621d1c53a450964880815128a24abcf25fddd3252bdd68f0c39dd8a17e0191d37bdd4bc0685a295b83b0781436e12ae272be@node-ug.dchain.id:30305,enode://82179cf70a8cec6096867a86edbddd79aac7cb651586ff123ad58f2cb26fdaa67784e903c8e9a0ae9ea4a483cb81d19bf5227b43e8e3438b154d4ed27880fefc@node-ut.dchain.id:30305,enode://fc32005fc49d4940701a4ce77bdc06cc2d1c47da30a71ea5cd2789ac055418a7fbf6751a6c4d0f7460cb01431ed37cacefab99786fbced026958d43412db3759@node-ub.dchain.id:30305,enode://961ddf94040314bf6c3cb877c3724ab5d6bb83a159ce7bc3364c20723e26951514403d7b56c4deaf10a142cf91efab7d0e81c4bac2d2842f111d56909048d44c@node-ugm.dchain.id:30305,enode://837a6a464a1e3d050977dd8ce823e18b6ad8f21dc9dda60bd14825c5253a792bd45feb5b77f95a9f31a67dc93662e57f2706699bf31551304452c439ae43d3a5@node-itb.dchain.id:30305

   ```
4. Jalankan file start.sh dengan cara mengetikan command

   `bash start.sh`
5. Jika sudah berhasil dijalankan, selanjutnya bisa di cek pada https://monitoring.dchain.id/ . Jika node yang dibuat sudah tampil maka node berhasil dibuat.
