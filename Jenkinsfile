pipeline {
    agent any
    
    stages {
        stage('Préparation') {
            parallel {
                stage('Réglage des machines à café ☕') {
                    steps {
                        echo 'Machines à café en mode turbo !'
                        sh 'date'
                        sh 'echo "Café préparé à : $(date)"'
                    }
                }
                stage('Affûtage des crayons ✏️') {
                    steps {
                        echo 'Réglage de la pointe...'
                        sh 'ls -la'
                        sh 'echo "Crayons affûtés et prêts à l\'emploi !"'
                    }
                }
            }
        }
        
        stage('Build & Test') {
            parallel {
                stage('Construction 🏗️') {
                    steps {
                        echo 'Assemblage des briques du projet...'
                        sh 'echo "Démarrage du build..."'
                        sh 'pwd'
                        sh 'echo "Build terminé !"'
                    }
                }
                stage('Tests 🧪') {
                    steps {
                        echo 'Lancement des tests...'
                        sh 'echo "Initialisation des tests..."'
                        sh 'ls'
                        sh 'echo "Tests terminés, résultats disponibles."'
                    }
                }
            }
        }
        
        stage('Déploiement') {
            steps {
                echo 'Déploiement en cours...'
                sh 'echo "Déploiement lancé à : $(date)"'
                sh 'echo "Déploiement terminé !"'
                echo 'Attention, la fusée est en route ! 🚀💥'
                echo 'Ça va secouer, mais ça va bien se passer... peut-être. 😅'
            }
        }
        
        stage('Notification & Célébration') {
            steps {
                echo 'Envoi des invitations à la fête de déploiement...'
                sh 'echo "Notifications envoyées à : $(date)"'
                echo 'La fête commence maintenant ! 🎉🎈'
                echo 'Chacun apporte son bug le plus bizarre... 🐛'
            }
        }
    }
}
