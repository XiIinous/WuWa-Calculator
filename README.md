# WuWa-Calculator

Wuthering Waves Damage Calculator
    Examples
        https://gidmgcalculator.web.app/
        https://genshin.aspirine.su/
            Possibly the addition of an optimizer (similar to https://frzyc.github.io/genshin-optimizer/)
            
Steps(?)
    Planning basic functions (calculator, inventory, resonators/characters [stats, scalings, etc…], Echoes [set bonuses, valid stats, sub/main interaction], weapons [passives, stats], Enemy stats, outside buffs, team buffs)
    Website Mockup
    Actual development/deployment
        Testing
        Debugging
        Revision
        
Resources (game)
    https://wutheringwaves.fandom.com/wiki/Wuthering_Waves_Wiki (genshin wiki   has the damage formula, so I assume wuwa will too)
    https://wutheringlab.com/ (has detailed information regarding stats, scalings, etc…)
    * Will probably be doing some actual testing in-game to check if damage values are correct, though most of how this will be checked will be using values after the target’s defense, buffs, debuffs, and resistances have been factored in. I’ll probably also be doing co-op a lot so I can see if there’s any changes to the base values (which genshin does) in vs out of co-op.
    
Timeline (Starting May 23, 2024)
    Week 1 (5/23-5/26):
        Get familiar with the mechanics and consider mechanics that weren’t previously considered
    Week 2 (5/27-6/2)
        Website mockup, test formulas
    Week 3 (6/3-6/9)
        Implement basic UI and functions. 
        Formulas will probably be for raw damage at this point
        Echo effects (for both main and sub slots)
    Week 4 (6/10-6/16)
        Implement other factors into the formulas (defense, resistances, debuffs, buffs [excluding team, including other]).
        Probably figure out how these can be toggled and adjusted by the user.
    Week 5 (6/17-6/23)
        Implement Team Composititons
            Figuring out how to factor in team-based buffs and debuffs, limited only to what those selected characters (and their gear) can provide
            
Other Considerations
    Constellation buffs 
        These are buffs gained by pulling dupes of characters/items
    Damage Optimizer 
        Direct Damage comparison between equipped and theoretical sets? Or between multiple manually configured sets/teams
        For teams this would mean making a calculator for damage per rotation as well. Probably excluding other team members’ damage in favor of focusing on the main DPS. The rotation will probably just be manually configured (user chooses how many instances of an attack/which attacks are used, buff initial activation frame, etc…)
    ^^^ Rotation calculator
        Should be easy as long as the regular calculator works
        If going very in depth–going to need average attack speed of each character and their skills to see how long buffs last and for which instances of damage, as well as how attack speed increases would factor into this.
        This assumes uninterrupted rotation 
    Snapshotting damage
        This one will probably require manual testing. For genshin, characters like XL could snapshot Q but XQ isn’t able to. Yelan isn’t able to snapshot either but has a global damage buff for team members that increases only for only the duration of the Q, and resets upon reactivation.
        Crit only vs. non crit vs. average damage
        Valid Stat Values
