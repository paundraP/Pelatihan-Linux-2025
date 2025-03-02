1. Membuat folder dan masuk kedalamnya
```bash
mkdir artists_who_can_sing && cd artists_who_can_sing
```
2. Download file zip menggunakan wget
```bash
wget --no-check-certificate 'https://drive.google.com/uc?export=download&id=1lV1HVmPTY_BOAK6ToXymRu7V5eVfR0ut' -O tutorials.zip
```
3. Unzip file yang sudah didownload dan dimasukkan ke folder baru
```bash
unzip tutorials.zip -d singing_tutorials
```
4. Menampilkan seluruh file
```bash
ls -la
```
5. Mencari flag part 1
```bash 
find . -type f -iname "*opera*NBAYoungboy*" -exec grep -i "FLAG" {} \; > ../flag.txt
```
6. Download file dari link yang didapatkan di flag
```bash
wget -O plsrunmeiamnotmalwarefr https://its.id/m/Arm64Alternative --no-check-certificate
```
7. Change permission terhadap file yang baru saja didownload sehingga dapat dijalankan
```bash
chmod +x plsrunmeiamnotmalwarefr
```
8. Menjalankan binary
```bash
./plsrunmeiamnotmalwarefr
```
9. Membuat file untuk menghentikan binary yang sudah dijalankan
```bash
touch ransom.moolah
```
10. Mematikan binary
```bash
Ctrl+C
```
11. Membuat sebuah user dan memasukkannya kedalam sudoers group
```bash
sudo sysadminctl -addUser yabadabadoo -password pujo && dseditgroup -o edit -a yabadabadoo -t user admin && su - yabadabadoo
```
12. Membuat direktori dan yang bisa mengakses hanya root dan yabadabadoo
```bash
sudo install -d -m 770 -o yabadabadoo -g wheel fufufafa
```
13. Solve puzle dan memasukkan ke folder fufufafa
```bash
find /tmp/pls_solve_this_puzzle -type f -name "hello_*.html" -exec sh -c 'tail -n1 "$1"' _ {} \; | grep -v '00000000: 0000 0000 0000 0000 0000 0000 0000 0000' | sort | cut -d' ' -f2- | tr -d ' ' | xxd -r -p | awk '{printf "%s", $0}' > fufufafa/flag2.txt
```
14. Menyalin flag.txt di user awal ke folder fufufafa milik yabadabadoo
```bash
sudo cp flag.txt /Users/yabadabadoo/fufufafa/
```
15. Delete folder yang ada di /tmp
```bash
sudo rm -rf /tmp/pls_solve_this_puzzle
```
