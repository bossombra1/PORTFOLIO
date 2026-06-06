<template>
    <section class="text-white mt-18" id="about">
        <!-- Effet lumineux en arrière-plan -->
        <div class="absolute z-0 top-[93rem] inset-x-0 h-64 flex items-start">
            <div class="h-24 w-64 bg-gradient-to-br from-primary via-secondary blur-2xl to-[#570cac] opacity-20"></div>
        </div>
        
        <!-- Grille principale sur deux colonnes (Texte à gauche, Image à droite) -->
        <div class="grid grid-cols-1 md:grid-cols-12 gap-8 items-center py-8 px-4 xl:gap-16 sm:py-16 xl:px-16 relative z-10">
            
            <!-- COLONNE GAUCHE : Textes et Compteurs  -->
            <div data-aos="fade-right" class="md:col-span-7 flex flex-col justify-between">
                <h2 class="text-4xl font-bold text-white text-left mb-6">
                    En savoir <span class="text-green-500">plus sur moi</span>
                </h2>
                
                <div class="space-y-4 text-base lg:text-lg text-gray-300 leading-8 mb-8">
                    <p>
                        Passionné par l'informatique et les nouvelles technologies, je suis un développeur d'applications junior avec une  formation en programmation et en gestion des systèmes informatiques. 
                    </p>
                    <p>
                        Créatif, rigoureux et curieux, j'ai acquis une précieuse expérience pratique au <strong>Ministère de la Défense</strong> où j'ai conçu des applications de gestion et de suivi de pensions critiques pour l'administration.
                    </p>
                </div>

                <!-- Les 3 petites cartes/compteurs du bas -->
                <div class="grid grid-cols-3 gap-4">
                    <!-- Carte 1 -->
                    <div class="bg-[#111a3e] border border-[#1f1641] rounded-2xl p-4 text-center shadow-lg">
                        <h3 class="text-2xl lg:text-3xl font-bold text-green-500">+3</h3>
                        <p class="text-xs lg:text-sm text-gray-400 uppercase tracking-wider mt-1">Technologies</p>
                    </div>
                    <!-- Carte 2 -->
                    <div class="bg-[#111a3e] border border-[#1f1641] rounded-2xl p-4 text-center shadow-lg">
                        <h3 class="text-2xl lg:text-3xl font-bold text-green-500">+3</h3>
                        <p class="text-xs lg:text-sm text-gray-400 uppercase tracking-wider mt-1">Applications</p>
                    </div>
                    <!-- Carte 3 -->
                    <div class="bg-[#111a3e] border border-[#1f1641] rounded-2xl p-4 text-center shadow-lg">
                        <h3 class="text-2xl lg:text-3xl font-bold text-green-500">Stage</h3>
                        <p class="text-xs lg:text-sm text-gray-400 uppercase tracking-wider mt-1">Expérience</p>
                    </div>
                </div>
            </div>

            <!-- COLONNE DROITE : L'image  -->
            <div data-aos="fade-left" class="md:col-span-5 flex justify-center mt-8 md:mt-0">
                <div class="relative w-72 h-72 sm:w-80 sm:h-80 lg:w-96 lg:h-96">
                    <!-- Cercle de fond coloré  -->
                    <div class="absolute inset-0 bg-green-600 rounded-full overflow-hidden border-2 border-green-500 shadow-2xl custom-profile-shape">
                        <!-- Ma photo  -->
                        <img src="@/assets/moi.jpeg" alt="Regis Kouame" class="w-full h-full object-cover object-top pt-4" />
                    </div>
                    <!-- Petit cercle de contour décoratif décalé visible  -->
                    <div class="absolute inset-0 border border-green-500 rounded-full transform translate-x-2 translate-y-2 pointer-events-none opacity-50"></div>
                </div>
            </div>

        </div>
    </section>
</template>

<style scoped>
/* Pour donner une forme légèrement asymétrique  */
.custom-profile-shape {
    border-radius: 42% 58% 70% 30% / 45% 45% 55% 55%;
}
</style>