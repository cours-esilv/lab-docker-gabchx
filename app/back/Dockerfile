# Étape 1 : Spécifiez l'image de base
FROM python:3.8

# Étape 2 : Définissez le répertoire de travail dans le conteneur
WORKDIR /app

# Étape 3 : Copiez le fichier requirements.txt dans le conteneur
COPY requirements.txt .

# Étape 4 : Installez les dépendances
RUN pip install -r requirements.txt

# Étape 5 : Copiez le reste du code de l'application dans le conteneur
COPY . .

# Étape 6 : Définissez la commande à exécuter lorsque le conteneur est lancé
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0"]