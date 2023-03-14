<script>
    import celeste from '../../assets/Gaming/celeste.png';
    import holllowknight from '../../assets/Gaming/holllowknight.png';
    import revelations from '../../assets/Gaming/revelations.png';
    import cuphead from '../../assets/Gaming/cuphead.png';
    import grumps from '../../assets/Gaming/grumps.png';
    import mario from '../../assets/Gaming/mario.png';

    const achievements = [
        { name: 'Thanks for playing', description: '"Complete every C-Side." - Celeste', image: celeste, alt: "celeste achievement", comment: 'This achievement covers, the completition of the main game, the B sides, and all C sides. This was a nightmare, but taught me patience.'},
        { name: 'The Hollow Knight', description: '"Defeat the Hollow Knight and become the Vessel." - Hollow Knight', image: holllowknight, alt: "hollow knight achievement", comment: 'The sacrifice of the Knight to contain the abyss.'},
        { name: 'A Better Tomorrow', description: '"In Revelations, complete the cycle. - Call Of Duty Black ops III"', image: revelations, alt: "call of duty bo3 achievement", comment: "A super easter egg that requires the completition of all BlackOps III zombies easter eggs."},
        { name: 'Souls Saved', description: '"Complete the game on Normal. - Cuphead"', image: cuphead, alt: "cuphead achievement", comment: "Completing the entire game on normal difficulty is quite a challenge, can't imagine on Expert mode."},
        { name: 'Metamorphosis', description: '"Rescue all of the imprisoned grubs. - Hollow Knight"', image: grumps, alt: "hollow knight achievement", comment: "Rescuing all the grubs, made me feel like a hero. Can't get over that final twist."},
        { name: 'Archivist Toadette', description: '"Aquire all the moons. - Mario Oddyssey"', image: mario, alt: "mario odyssey achievement", comment: "One of the most enjoyable game experiences I've ever had."},
    ]
</script>

<div class="theme-container mt-20">
    <div class="mx-auto max-w-2xl items-center gap-x-8 px-4 sm:px-6 py-8 lg:max-w-7xl lg:grid-cols-2 lg:px-8">
        <div id="games-achievements">
            <h2 class="text-3xl font-bold tracking-tight sm:text-4xl">My Proudest Archievements</h2>
            <p class="mt-4">
                These are some of the best moments I've ever had playing videogames. 
                Some are just really hard archievements to get, and some are just there because they hold a special place in my heart
            </p>

            <dl class="mt-16 grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 sm:gap-y-16 lg:gap-x-8">
                {#each achievements as achievement}
                    <div key={achievement.name} class="border-t border-gray-200 pt-4">
                        <img src={achievement.image} alt={achievement.alt} width='64px' height='64px'/>
                        <dt class="font-medium mt-4">{achievement.name}</dt>
                        <dd class="mt-2 text-smb theme-color-accent font-semibold">{achievement.description}</dd>
                        <dd class="mt-2 text-sm">{achievement.comment}</dd>
                    </div>
                {/each}
            </dl>
        </div>
    </div>
</div>