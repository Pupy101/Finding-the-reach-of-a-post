# Finding the reach of a post

### Задача была решена в рамках 24 часового хакатона.
![image](https://drive.google.com/file/d/1i5LzBHoOvaFzxVtaQMsuHw2K3XMk2NUr/view?usp=sharing)

### В качестве формулы охвта используется следующее выражение:
![image](https://drive.google.com/file/d/19p91hvYCVZnrk0fXgW8gMEiwaOdgMrB1/view?usp=sharing)

### Основой модели был выбран Берт, выдававший вектроное представление предложения.
![image](https://drive.google.com/file/d/1XsX4_Ak3HT_D60dTpP3j0SgmFSGTyUhq/view?usp=sharing)
### На этой основе была располжена лстм, которая в зависимости от подаваемого токена дня недели возвращала выход и полученное скрытое представление.
![image](https://drive.google.com/file/d/1aEtqUBHLLSeRn4-UanGRugTUocrCmZhM/view?usp=sharing)
### Последним уровнем модели были обычные полносвязные линейные слои с активацией ReLU и Dropout.

### Исходные данные были проанализированны, почищенны от неинформативных примеров, отнормированны и разелены на train/test. Более подробно можно увидеть в ноутбуке.

### Абсолютная разница между спрогнозируемым охватом и реальным на валидационной выборке составила 0.0025
