# UltimateChemCalc
PYPI Package containing chemistry related calculators that cover basic mole conversions, stoichiometry, chemical equation balancing, and molarity...

# Overview
Documentation for all conversion and balancing functions (non-user Interface Version):

# 0. Version 3.0 Addition:
     This new version includes a new feature within the graphical version. The graphical version now has a new alpha version balancer that
     can balance equations in acidic/basic solutions. Do note though that this feature is in the ALPHA phase, and so some kinks are still being
     worked out, and an additional feature will be added within the next version that will get rid of these kinks (an oxidation number solver).
     Until most of the kinks are worked out though, the old chemical equation balancer will be associated with the getEquation() function. Within
     the graphical version, the old chemical equation balancer is also provided through the Normal Balance Button...

# 1. Basic Mole Conversions:

   How to use:<br/>
       from UltimateChemCalc import FUNCTION_NAME

   ## def gramToMole(gram,molarMass)<br/>
       +Covert from grams to moles...
    		+gram = The given grams amount.
    		+molarMass = The molar mass of the elment or molecule in question.

   ## def gramToMoleToParticle(gram,molarMass)
       +Convert from grams to particles...
       		+gram = The given grams amount.
		    	+molarMass = The molar mass of the element or molecule in question.

   ## def gramToMoleToParticleToAtom(gram,molarMass,atoms)
       +Convert from grams to atoms...
       		+gram = The given grams amount.
			+molarMass = The molar mass of the molecule in question.
			+atoms = The subscript associated with a particular element within
		         	 the moecule.

   ## def moleToGram(moles,molarMass)
       +Convert from moles to grams...
       		+moles = The given moles amount.
			+molarMass = The molar mass of the element or molecule in question.

   ## def moleToParticle(moles)
       +Convert from moles to particles...
       		+moles = The given moles amount.

   ## def moleToMoleculeToAtom(moles,atoms)
       +Convert from moles to atoms...
       		+moles = The given moles amount.
			+atoms = The subscript associated with a particular element within
		         	 the molecule.

   ## def moleculeToAtom(molecule,atoms)
       +Convert from molecules to atoms...
       		+molecule = The given molecules amount.
			+atoms = The subscript associated with a particular element within
		         	 the molecule.

   ## def particleToMole(particle)
       +Convert from particles to moles...
       		+particle = The givn particles amount.

   ## def particleToGram(particle,molarMass)
       +Convert from particles to grams...
       		+particle = The given particles amount.
			+molarMass = The molar mass of the element or molecule in question.

   ## def LiterToGram(liter,molarMass)
       +Convert from liters to grams...
       		+liter = The given liters amount (gas at STP).
			+molarMass = The molar mass of the element or molecule in question.

   ## def LiterToParticle(liter)
       +Convert from liters to particles...
       		+liter = The given liters amount (gas at STP).

   ## def LiterToAtom(liter,atom)
       +Convert from liters to atoms...
      	       +liter = The given liters amount (gas at STP).
	       		+atom = The subscript associated with a particular element within
	               		the molecule.

   ## def MoleToLiter(mole)
       +Convert from moles to liters (gas at STP)...
       		+mole = The given moles amount.

   ## def LiterToMole(liter)
       +Convert from liters to moles...
       		+liter = The given liters amount (gas at STP).

   ## def GramToLiter(gram,molarMass)
       +Convert from grams to liters (gas at STP)...
       		+gram = The given grams amount.
			+molarMass = The molar mass of the element or molecule in question.

   ## def ParticleToLiter(particles)
       +Convert from particles to liters (gas at STP)...
       		+particles = The given particles amount.

# 2. Stoichiometry Conversion Problems

How to use:<br/>
       from UltimateChemCalc import FUNCTION_NAME
       
       
   ## def MoleToMole(given,mole1,mole2)
       +Convert from moles to moles...
       		+given = The given moles amount.
			+mole1 = The mole amount of the known substance.
			+mole2 = The mole amount of the unknown substance.

   ## def SGramToGram(given,molarMass,known,unknown,molarMass2)
       +Convert from grams to grams...
       		+given = The given grams amount.
			+molarMass = The molar mass of the known substance.
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.
			+molarMass2 = The molar mass of the unknown substance.

   ## def SGramToMole(gram,molarMass,known,unknown)
       +Convert from grams to moles...
       		+gram = The given grams amount.
			+molarMass = The molar mass of the known substance.
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.


   ## def GramToParticle(gram,molarMass,known,unknown)
       +Convert from grams to particles...
       		+gram = The given grams amount.
			+molarMass = The molar mass of the known substance.
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.

   ## def SGramToAtom(gram,molarMass1,known,unknown,atoms)
       +Convert from grams to atoms...
       		+gram = The given grams amount.
			+molarMass1 = The molar mass of the known substance.
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.
			+atoms = The subscript associated with an element within the unknown substance.

   ## def SGramToLiter(gram,molarMass,known,unknown)
       +Convert from grams to liters...
       		+gram = The given grams amount.
			+molarMass = The molar mass of the known substance.
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.

   ## def SMoleToGram(mole,known,unknown,molarMass)
       +Convert from moles to grams...
       		+mole = The given moles amount.
		+known = The moles amount of the known substance.
		+unknown = The moles amount of the unknown substance.
		+molarMass = The molar mass of the unknown substance.

   ## def SMoleToParticle(mole,known,unknown)
       +Convert from moles to particles...
       		+mole = The given moles amount.
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.

   ## def SMoleToAtoms(mole,known,unknown,atoms)
       +Convert from moles to atoms...
       		+mole = The given moles amount.
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.
			+atoms = The subscript associated with an element of the unknown substance.

   ## def SMoleToLiter(mole,known,unknown)
       +Convert from moles to liters (gas at STP)...
       		+mole = The given moles amount.
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.

   ## def SParticleToGram(particle,known,unknown,molarMass)
       +Convert from particles to grams...
       		+particle = The given particles amount.
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.

   ## def SParticleToMole(particle,known,unknown)
       +Convert from particles to moles...
       		+particle = The given particles amount.
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.

   ## def SParticleToParticle(particle,known,unknown)
       +Convert from particles to particles...
       		+particle = The given particles amount.
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.

   ## def SParticleToAtom(particle,known,unknown,atom)
       +Convert from particles to atoms...
       		+particle = The given particles amount.
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.
			+atom = The subscript associated with an element of the unknown substance.

   ## def SParticleToLiter(particle,known,unknown)
       +Convert from particles to liters...
       		+particle = The given particles amount.
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.

   ## def SLiterToGram(liter,known,unknown,molarMass)
       +Convert from liters to grams...
       		+liter = The given liters amoount (gas at STP).
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.
			+molarMass = The molar mass of the unknown substance.

   ## def SLiterToMole(liter,known,unknown)
       +Convert from liters to moles...
       		+liter = The given liters amoount (gas at STP).
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.

   ## def SLiterToParticle(liter,known,unknown)
       +Convert from liters to particles...
       		+liter = The given liters amoount (gas at STP).
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.

   ## def SLiterToAtom(liter,known,unknown,atoms)
       +Convert from liters to atoms...
       		+liter = The given liters amoount (gas at STP).
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.
			+atoms = The subscript associated with an element of the unknown substance.

   ## def SLiterToLiter(liter,known,unknown)
       +Convert from liters to liters...
       		+liter = The given liters amoount (gas at STP).
			+known = The moles amount of the known substance.
			+unknown = The moles amount of the unknown substance.

# 3. Molarity Conversion Problems

   How to use:
       from UltimateChemCalc import FUNCTION_NAME

   ## def LiquidLiterToMole(liter,molarL)
       +Convert from liters to moles (Liquids)...
       		+liter = The given liters amount.
			+molarL = The molarity (# liters / 1 Mole).

   ## def LiquidLiterToGram(liter,molarL,molarMass)
       +Convert from liters to grams (Liquids)...
       		+liter = The given liters amount.
			+molarL = The molarity (# liters / 1 Mole).

   ## def LiquidLiterToParticles(liter,molarL)
       +Convert from liters to particles (Liquids)...
       		+liter = The given liters amount.
			+molarL = THe molarity (# liters / 1 Mole).

# 4. Chemical Equation Balancing

   How to use:<br/>
       from UltimateChemCalc import getEquation

   ## def getEquation()
       +Provide an unbalanced chemical equation and get back
        a balanced version. (The provided chemical equation must have no coefficients)
	  	+The program will prompt the user for input...
       			+Don't Use Spaces!
       +Example Equation: H2+O2->H2O
       +Example Equation: H2O+CrO4[-2]+SO3[-2]->Cr(OH)3+SO4[-2]+OH[-1]

# 5. Graphical-Calculator

  How to use: <br/>
      from UltimateChemCalc import startG

  ## def startG()
      +Launch the graphical desktop application containing every chemistry calculator within
       this documentation...

  ## Warning!
     +If using apple OS, you must use pythonw...