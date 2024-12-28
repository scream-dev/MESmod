# MESmod
## Мод на МЭШ делающийся энтузиастом, чтобы логиниться по Логину и Паролю

## Для FireFox:
Получить токен:
function getCookie(name) {
    const value = `; ${document.cookie}`;
    const parts = value.split(`; ${name}=`);
    if (parts.length === 2) return parts.pop().split(';').shift();
}

const token = getCookie('aupd_token');

if (token) {
    console.log(`Вот токен вашего МЭШ: ${token}`);
} else {
    console.log("Токен не найден. Проверьте, вошли ли вы в дневник сейчас, это обязательно для получения токена.");
}

