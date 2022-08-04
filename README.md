# stellar-lifespan

A calculator for stellar main sequence lifespans, allowing users to adjust stellar mass and luminosity (both relative to the sun).  This is a super-simplified approximation, treating the amount of core hydrogen as proportional to stellar mass.  In the "realistic" mode, it uses the M^4 relation for luminosity which is a reasonable approximation for a large range of stellar masses, but breaks down at low and high masses.  

The format is designed for embedding within the stream of reading, so specifically formatted to be wide and short.  

It also supports URL parameters for pedagogically specific use cases.  To use an option when preparing the URL for students, add ? followed by parameters.  Multiple parameters can be given by joining them with &

realistic=true       starts the simulation in the mode where luminosity is a function of mass
mass=NUMBER          specify a starting mass
luminosity=NUMBER    specify a starting mass
fixedMass=true       lock the mass
fixedLuminosity=true lock the luminosity

For example, to have students explore the effect of mass alone on the stellar lifespan, provide the link:
  https://foothillastrosims.github.io/stellar-lifespan/index.html?fixedLuminosity=true
  
To embed in a web page, use the following HTML:
  <p><iframe src="https://foothillastrosims.github.io/stellar-lifespan/index.html" width="100%" height="210px"></iframe></p>
