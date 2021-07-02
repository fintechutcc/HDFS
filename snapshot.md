# การสร้าง Snapshot บน HDFS

## 1. ล็อกอินด้วยบัญชี hdfs
su -u hdfs

## 2. อนุญาตให้สร้าง Snapshot
```
hdfs dfsadmin -allowSnapshot <path>
```

## 3. สร้าง Snapshot
เมื่ออนุญาตให้สร้าง Snapshot ในโฟลเดอร์ที่ต้องการแล้ว สามารถใช้บัญชีใด ๆ ในการสร้าง Snapshot ของโฟลเดอร์นั้น คำสั่งที่ใช้ในการสร้าง Snapshot คือ
```
hdfs dfs -createSnapshot <path> [<snapshotName>]
```