# FreqScalper 🚀

FreqScalper est un bot de trading automatisé basé sur **Freqtrade**, conçu pour optimiser le scalping et l'exécution de stratégies avancées sur les marchés crypto. 

## 📌 Fonctionnalités principales

✅ **Stratégies dynamiques** : RSI, MACD, SuperTrend, Ichimoku et plus encore.  
✅ **Gestion avancée du risque** : Stop-loss, take-profit et trailing stop.  
✅ **Backtests et optimisations** : Simulation et ajustement des stratégies.  
✅ **Intégration Telegram** : Alertes en temps réel et suivi des trades.  
✅ **Déploiement Dockerisé** : Configuration et exécution simplifiées.  
✅ **Support PostgreSQL** : Gestion efficace de plusieurs bots simultanément.

---

## 🚀 Installation & Configuration

### 1️⃣ Cloner le dépôt
```bash
git clone https://github.com/ton-utilisateur/FreqScalper.git
cd FreqScalper
```

### 2️⃣ Installer les dépendances
Assurez-vous d'avoir Python 3.8+ et installez Freqtrade :
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

### 3️⃣ Configurer le bot
Générez un fichier de configuration initial :
```bash
freqtrade new-config --config config.json
```
Adaptez les paramètres dans `config.json` selon vos besoins.

### 4️⃣ Lancer un backtest
```bash
freqtrade backtest --config config.json --strategy MaStrategie
```

### 5️⃣ Démarrer le bot en mode live
```bash
freqtrade trade --config config.json --strategy MaStrategie
```

---

## 📊 Stratégies incluses

- `ScalpRSIMacd` : Scalping basé sur RSI et MACD.
- `SuperTrendMomentum` : Détection des tendances avec SuperTrend.
- `IchimokuBreakout` : Signal d'entrée basé sur Ichimoku.

Vous pouvez ajouter vos propres stratégies dans le dossier `user_data/strategies/`.

---

## 🔥 Déploiement avec Docker

Si vous préférez utiliser Docker :
```bash
docker-compose up -d
```
Adaptez le fichier `docker-compose.yml` selon vos besoins.

---

## 📢 Alertes Telegram

Activez les alertes Telegram en configurant votre bot dans `config.json` :
```json
"telegram": {
    "enabled": true,
    "token": "VOTRE_TOKEN",
    "chat_id": "VOTRE_CHAT_ID"
}
```

---

## 📜 Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.

---

## 🤝 Contribution

Les contributions sont les bienvenues ! Créez une **issue** ou un **pull request** si vous avez des idées d'amélioration.

---

🚀 **Bonne stratégie et bon trading !** 🚀
