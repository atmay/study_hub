# Запускаем Терминал

- Command+Пробел -> вводим Terminal


# Устанавливаем пакетного менеджера homebrew

Для macOS существует пакетный менеджер Homebrew. Удобно устанавливать через него программы и управлять ими.

https://brew.sh

Вводим команду с главной страницы в терминал:

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"


Добавляем пакетный менеджер Homebrew к переменным окружения. По очереди вводим в терминал команды:

```
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)" 
```

# Устанавливаем Python

Сначала смотрим, какие версии Python уже есть. В терминале вводим:

```
brew search python 
```

По умолчанию в macOS уже установлен Python. Установленная версия будет отмечена галочкой.
Устанавливаем свежую версию:
```
brew install python@3.11
```

Смотрим, как версия стоит по умолчанию:

```
python3 --version 
```

Переназначить версию по умолчанию:
```
brew unlink python@3.<current>
brew link python@3.11
```
