Задание I
1. Фронтенд разбит 4 проекта: 
  a. host - точка входа
	host\src\components\App.js - точка входа
  b. photo - микрофронтенд. Управление фотографиями
	photo-microfrontend\src\components\AddPlacePopup.js - компонент добавление фотографии
	photo-microfrontend\src\components\Card.js - компонент карточки фотографии
	photo-microfrontend\src\components\ImagePopup.js - всплывающее окно с фотографией
	photo-microfrontend\src\components\PopupWithForm.js - всплывающее окно с формой
  c. profile -микрофронтенд. Управление профилем пользователя
	profile-microfrontend\src\components\EditProfilePopup.js - компонент управления профилем пользователя
	profile-microfrontend\src\components\EditAvatarPopup.js - компонент управления аватара пользователя
  d. auth - микрофронтенд. Аутентификация и регистрация.
	auth-microfrontend\src\components\login.js  - компонент входа пользователя в систему
	auth-microfrontend\src\components\register.js - компонент регистрации пользователя в систему
	auth-microfrontend\src\components\InfoTooltip.js - всплывающее диалоговое окно
	 
	

Для декомпозиции проекта был выбран подход WebPack Module Federation, т.к. во всех под проектах используется один фреймворк React.
Была использована стратегия  "вертикальной нарезки". Были выделены домены домены - аутентификация, управление фотографиями, управление профилем пользователя.

Запуск проекта: 
	docker compose -f 'compose.yaml' up -d --build

PS. Выполнены только 2 уровня первого задания.

Задание II
https://drive.google.com/file/d/1PF0TV3s3HTMSwUtU8CzLHVHIOQWg7Vw3/view?usp=drive_link