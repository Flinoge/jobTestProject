<template>
  <div id="container">
	    
	    <div id="header">
	    	<h1>Periodic Table</h1>
	    </div>
	    
	    <div id="sidebar">
			<div id="legend">
				<h2>Legend</h2>
				<p class="border">Metals</p>
				<p>A solid substance that is a good cborderonductor of eat and electicity. Can be formed into many shapes.</p>
				
				<p class="border metalloidsImportant">Metalloid</p>
				<p>"Middle elements" - conduct heat and electricity better than nonmetals, 
					but not as well as metals. Easier to shape than nonmetals, but not as easy as metals.  
					Solid at room temperature.</p>
			
				<p  class="border nonmetalsImportant">Nonmetals</p>
				<p>A poor conductor of heat and electricity.  Not easily formed into shapes.</p>
			</div>
	    </div>
	    
	    <div id="content">
	    	<h2>Elements</h2>
	    	<table id="periodic">
	    		<tr>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.H)">H</td>
	    			<td class="white" colspan="16"></td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.He)">He</td>
	    		</tr>
	    		<tr>
	    			<td @click="clickElement(elements.Li)">Li</td>
	    			<td @click="clickElement(elements.Be)">Be</td>
	    			<td class="white" colspan="10"></td>
	    			<td class="metalloidsImportant" @click="clickElement(elements.B)">B</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.C)">C</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.N)">N</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.O)">O</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.F)">F</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.NE)">Ne</td>
	    		</tr>
	    		<tr>
	    			<td @click="clickElement(elements.Na)">Na</td>
	    			<td @click="clickElement(elements.Mg)">Mg</td>
	    			<td class="white" colspan="10"></td>
	    			<td @click="clickElement(elements.Al)">Al</td>
	    			<td class="metalloidsImportant" @click="clickElement(elements.Si)">Si</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.P)">P</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.S)">S</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.Cl)">Cl</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.Ar)">Ar</td>
	    		</tr>
	    		<tr>
	    			<td @click="clickElement(elements.K)">K</td>
	    			<td @click="clickElement(elements.Ca)">Ca</td>
	    			<td @click="clickElement(elements.Sc)">Sc</td>
	    			<td @click="clickElement(elements.Ti)">Ti</td>
	    			<td @click="clickElement(elements.V)">V</td>
	    			<td @click="clickElement(elements.Cr)">Cr</td>
	    			<td @click="clickElement(elements.Mn)">Mn</td>
	    			<td @click="clickElement(elements.Fe)">Fe</td>
	    			<td @click="clickElement(elements.Co)">Co</td>
	    			<td @click="clickElement(elements.Ni)">Ni</td>
	    			<td @click="clickElement(elements.Cu)">Cu</td>
	    			<td @click="clickElement(elements.Zn)">Zn</td>
	    			<td @click="clickElement(elements.Ga)">Ga</td>
	    			<td class="metalloidsImportant" @click="clickElement(elements.Ge)">Ge</td>
	    			<td class="metalloidsImportant" @click="clickElement(elements.As)">As</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.Se)">Se</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.Br)">Br</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.Kr)">Kr</td>
	    		</tr>
	    		<tr>
	    			<td @click="clickElement(elements.Rb)">Rb</td>
	    			<td @click="clickElement(elements.Sr)">Sr</td>
	    			<td @click="clickElement(elements.Y)">Y</td>
	    			<td @click="clickElement(elements.Zr)">Zr</td>
	    			<td @click="clickElement(elements.Nb)">Nb</td>
	    			<td @click="clickElement(elements.Mo)">Mo</td>
	    			<td @click="clickElement(elements.Tc)">Tc</td>
	    			<td @click="clickElement(elements.Ru)">Ru</td>
	    			<td @click="clickElement(elements.Rh)">Rh</td>
	    			<td @click="clickElement(elements.Pd)">Pd</td>
	    			<td @click="clickElement(elements.Ag)">Ag</td>
	    			<td @click="clickElement(elements.Cd)">Cd</td>
	    			<td @click="clickElement(elements.In)">In</td>
	    			<td @click="clickElement(elements.Sn)">Sn</td>
	    			<td class="metalloidsImportant" @click="clickElement(elements.Sb)">Sb</td>
	    			<td class="metalloidsImportant" @click="clickElement(elements.Te)">Te</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.I)">I</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.Xe)">Xe</td>
	    		</tr>
	    		<tr>
	    			<td @click="clickElement(elements.Cs)">Cs</td>
	    			<td @click="clickElement(elements.Ba)">Ba</td>
	    			<td @click="clickElement(elements.La)">La</td>
	    			<td @click="clickElement(elements.Hf)">Hf</td>
	    			<td @click="clickElement(elements.Ta)">Ta</td>
	    			<td @click="clickElement(elements.W)">W</td>
	    			<td @click="clickElement(elements.Re)">Re</td>
	    			<td @click="clickElement(elements.Os)">Os</td>
	    			<td @click="clickElement(elements.Ir)">Ir</td>
	    			<td @click="clickElement(elements.Pt)">Pt</td>
	    			<td @click="clickElement(elements.Au)">Au</td>
	    			<td @click="clickElement(elements.Hg)">Hg</td>
	    			<td @click="clickElement(elements.Tl)">Tl</td>
	    			<td @click="clickElement(elements.Pb)">Pb</td>
	    			<td @click="clickElement(elements.Bi)">Bi</td>
	    			<td @click="clickElement(elements.Po)">Po</td>
	    			<td class="metalloidsImportant" @click="clickElement(elements.At)">At</td>
	    			<td class="nonmetalsImportant" @click="clickElement(elements.Rn)">Rn</td>
	    		</tr>
	    		<tr>
	    			<td @click="clickElement(elements.Fr)">Fr</td>
	    			<td @click="clickElement(elements.Ra)">Ra</td>
	    			<td @click="clickElement(elements.Ac)">Ac</td>
	    			<td @click="clickElement(elements.Unq)">Unq</td>
	    			<td @click="clickElement(elements.Unp)">Unp</td>
	    			<td @click="clickElement(elements.Unh)">Unh</td>
	    			<td @click="clickElement(elements.Uns)">Uns</td>
	    			<td @click="clickElement(elements.Uno)">Uno</td>
	    			<td @click="clickElement(elements.Une)">Une</td>
	    			<td class="white" colspan="9"></td>
	    		</tr>
	    		<tr>
	    			<td @click="clickElement(elements.Ce)">Ce</td>
	    			<td @click="clickElement(elements.Pr)">Pr</td>
	    			<td @click="clickElement(elements.Nd)">Nd</td>
	    			<td @click="clickElement(elements.Pm)">Pm</td>
	    			<td @click="clickElement(elements.Sm)">Sm</td>
	    			<td @click="clickElement(elements.Eu)">Eu</td>
	    			<td @click="clickElement(elements.Gd)">Gd</td>
	    			<td @click="clickElement(elements.Tb)">Tb</td>
	    			<td @click="clickElement(elements.Dy)">Dy</td>
	    			<td @click="clickElement(elements.Ho)">Ho</td>
	    			<td @click="clickElement(elements.Er)">Er</td>
	    			<td @click="clickElement(elements.Tm)">Tm</td>
	    			<td @click="clickElement(elements.Yb)">Yb</td>
	    			<td @click="clickElement(elements.Lu)">Lu</td>
	    			<td class="white" colspan="4"></td>
	    		</tr>
	    		<tr>
	    			<td @click="clickElement(elements.Th)">Th</td>
	    			<td @click="clickElement(elements.Pa)">Pa</td>
	    			<td @click="clickElement(elements.U)">U</td>
	    			<td @click="clickElement(elements.Np)">Np</td>
	    			<td @click="clickElement(elements.Pu)">Pu</td>
	    			<td @click="clickElement(elements.Am)">Am</td>
	    			<td @click="clickElement(elements.Cm)">Cm</td>
	    			<td @click="clickElement(elements.Bk)">Bk</td>
	    			<td @click="clickElement(elements.Cf)">Cf</td>
	    			<td @click="clickElement(elements.Es)">Es</td>
	    			<td @click="clickElement(elements.Fm)">Fm</td>
	    			<td @click="clickElement(elements.Md)">Md</td>
	    			<td @click="clickElement(elements.No)">No</td>
	    			<td @click="clickElement(elements.Lr)">Lr</td>
	    			<td class="white" colspan="4"></td>
	    		</tr>
	    	</table>
	    	
	    	<div id="elementProperties"></div>  
	    </div>
	    <div id="footer">
	    	&copy;2013 Weber State University
	    </div>
    </div>
</template>

<script>
export default {
  name: 'hello',
  methods: {
    clickElement (el) {
      alert('Name: ' + el[0] + ' Number: ' + el[1] + ' Atomic Weight ' + el[2] + ' Melts: ' + el[3] + ' Freezes ' + el[4])
    },
    hoverElement (el) {
      document.getElementById('elementProperties').innerHTML = el
    }
  },
  data () {
    return {
      elements: {
        H: ['Hydrogen', '1', '1.0079', '-259.14C', '-252.87C'],
        He: ['Helium', '2', '4.0026', '-272C @ 26ATM', '-268.6C'],
        Li: ['Lithium', '3', '6.94', '180.54 C', '1347 C'],
        Be: ['Beryllium', '4', '9.01218', '1278 C', '2970 C'],
        B: ['Boron', '5', '10.81', '2300 C', '2550 C'],
        C: ['Carbon', '6', '12.011', '3500 C', '4827 C'],
        N: ['Nitrogen', '7', '14.0067', '-209.9 C', '-195.8 C'],
        O: ['Oxygen', '8', '15.9994', '-218.4 C', '-183.0 C'],
        F: ['Flourine', '9', '18.998403', '-219.62 C', '-188.14 C'],
        Ne: ['Neon', '10', '20.17', '-248.6 C', '-246.1 C'],
        Na: ['Sodium', '11', '22.98977', '97.8 C', '882.9 C'],
        Mg: ['Magnesium', '12', '24.305', '638.8 C', '1090 C'],
        Al: ['Aluminum', '13', '26.98154', '660.37 C', '2467 C'],
        Si: ['Silicon', '14', '28.0855', '1410 C', '2355 C'],
        P: ['Phosphorous', '15', '30.97376', '44.1 C', '280 C'],
        S: ['Sulfur', '16', '32.06', '112.8 C', '444.6 C'],
        Cl: ['Chlorine', '17', '35.453', '-100.98 C', '-34.6 C'],
        Ar: ['Argon', '18', '39.948', '-189.3 C', '-186 C'],
        K: ['Potassium', '19', '39.0983', '63.65 C', '774 C'],
        Ca: ['Calcium', '20', '40.08', '839 C', '1484.4 C'],
        Sc: ['Scandium', '21', '44.9559', '1539 C', '2832 C'],
        Ti: ['Titanium', '22', '47.90', '1660 C', '3287 C'],
        V: ['Vandium', '23', '50.9415', '1890±10 C', '3380 C'],
        Cr: ['Chromium', '24', '51.996', '1857 C', '2672 C'],
        Mn: ['Manganese', '25', '54.9380', '1245 C', '1962 C'],
        Fe: ['Iron', '26', '55.847', '1535 C', '2750 C'],
        Co: ['Cobalt', '27', '58.9332', '1495 C', '2870 C'],
        Ni: ['Nickel', '28', '58.71', '1453 C', '2732 C'],
        Cu: ['Copper', '29', '63.546', '1803 C', '2567 C'],
        Zn: ['Zinc', '30', '65.38', '419.58 C', '907 C'],
        Ga: ['Gallium', '31', '69.735', '29.78 C', '2403 C'],
        Ge: ['Germanium', '32', '72.59', '937.4 C', '2830 C'],
        As: ['Arsenic', '33', '74.9216', '81 C @ 28ATM', 'Sublimes at 613'],
        Se: ['Selenium', '34', '78.96', '217 C', '684.9 C'],
        Br: ['Bromine', '35', '79.904', '-7.2 C', '58.78 C'],
        Kr: ['Krypton', '36', '83.80', '-157.2 C', '-153.4 C'],
        Rb: ['Rubidium', '37', '85.467', '38.89 C', '688 C'],
        Sr: ['Strontium', '38', '87.62', '769 C', '1384 C'],
        Y: ['Yttrium', '39', '88.9059', '1523 C', '3337 C'],
        Zr: ['Zirconium', '40', '91.22', '1852±2 C', '4377 C'],
        Nb: ['Niobium', '41', '92.9064', '2468±10 C', '4927 C'],
        Mo: ['Molybdenum', '42', '95.94', '2617 C', '4612 C'],
        Tc: ['Technetium', '43', '98.9062', '2200±50 C', '4877 C'],
        Ru: ['Ruthenium', '44', '101.07', '2250 C', '3900 C'],
        Rh: ['Rhodium', '45', '102.9055', '1966±3 C', '3727 C'],
        Pd: ['Palladium', '46', '106.4', '1552 C', '2927 C'],
        Ag: ['Silver', '47', '107.868', '961.93 C', '2212 C'],
        Cd: ['Cadmium', '48', '112.41', '320.9 C', '765 C'],
        In: ['Indium', '49', '114.82', '156.61 C', '2000±10 C'],
        Sn: ['Tin', '50', '118.69', '231.9 C', '2270 C'],
        Sb: ['Antimony', '51', '121.75', '630 C', '1750 C'],
        Te: ['Tellurium', '52', '127.60', '449.5 C', '989.8 C'],
        I: ['Iodine', '53', '126.9045', '113.5 C', '184 C @ 35 atm'],
        Xe: ['Xenon', '54', '131.30', '-111.9 C', '-108.1 C'],
        Cs: ['Cesium', '55', '132.9054', '28.5 C', '678.4 C'],
        Ba: ['Barium', '56', '137.33', '725 C', '1140 C'],
        La: ['Lanthanum', '57', '138.9055', '920 C', '3469 C'],
        Hf: ['Hafnium', '72', '178.49', '2150 C', '5400 C'],
        Ta: ['Tantalum', '73', '180.947', '2996 C', '5425±100 C'],
        W: ['Tungsten', '74', '183.85', '3410±20 C', '5660 C'],
        Re: ['Rhenium', '75', '186.207', '3180 C', '5627 C'],
        Os: ['Osmium', '76', '190.2', '3045 C', '5027 C'],
        Ir: ['Iridium', '77', '192.22', '2410 C', '4527±100 C'],
        Pt: ['Platinum', '78', '195.09', '1772 C', '3827 C'],
        Au: ['Gold', '79', '196.9665', '1064.43 C', '2807 C'],
        Hg: ['Mercury', '80', '200.59', '-38.87 C', '356.58 C'],
        Tl: ['Thallium', '81', '204.37', '303.5 C', '1457±10C'],
        Pb: ['Lead', '82', '207.2', '327.5 C', '1740 C'],
        Bi: ['Bismuth', '83', '208.9804', '271.3 C', '1560±5C'],
        Po: ['Polonium', '84', '(209)', '254 C', '962 C'],
        At: ['Astatine', '85', '(210)', '302 C', '337 C'],
        Rn: ['Radon', '86', '(222)', '-71 C\t', '-61.8 C'],
        Fr: ['Francium', '87', '(223)', '27 C\t', '677 C'],
        Ra: ['Radium', '88', '226.0254', '700 C', '1737 C'],
        Ac: ['Actinium', '89', '(227)', '1050 C', '3200±300 C'],
        Unq: ['Unnilquadium', '104', '(260)', 'N/A C', 'N/A C'],
        Unp: ['Unnilpentium', '105', '(260)', 'N/A C', 'N/A C'],
        Unh: ['Unnilhexium', '106', '(263)', 'N/A C', 'N/A C'],
        Uns: ['Unnilseptium', '107', '(262)', 'N/A C', 'N/A C'],
        Uno: ['Unniloctium', '108', '(265)', ' N/A C', 'N/A C'],
        Une: ['Unnilennium', '109', '(267)', ' N/A C', 'N/A C'],
        Qe: ['Cerium', '58', '140.12', '795 C', '3257 C'],
        Pr: ['Praseodymium', '59', '140.9077', '935 C', '3127 C'],
        Nd: ['Neodymium', '60', '144.24', '1010 C', '3127 C'],
        Pm: ['Promethium', '61', '(145)', 'N/A C', 'N/A C'],
        Sm: ['Samarium', '62', '150.4', '1072 C', '1900 C'],
        Eu: ['Europium', '63', '151.96', '822 C', '1597 C'],
        Gd: ['Gadolinium', '64', '157.25', '1311 C', '3233 C'],
        Tb: ['Terbium', '65', '158.9254', '1360 C', '3041 C'],
        Dy: ['Dysprosium', '66', '162.50', '1412 C', '2562 C'],
        Ho: ['Holmium', '67', '164.9304', '1470 C', '2720 C'],
        Er: ['Erbium', '68', '167.26', '1522 C', '2510 C'],
        Tm: ['Thulium', '69', '168.9342', '1545 C', '1727 C'],
        Yb: ['Ytterbium', '70', '173.04', '824 C', '1466 C'],
        Lu: ['Lutetium', '71', '174.96', '1656 C', '3315 C'],
        Th: ['Thorium', '90', '232.0381', '1750 C', '4790 C'],
        Pa: ['Proactinium', '91', '231.0359', '1600 C', 'N/A C'],
        U: ['Uranium', '92', '238.029', '1132 C', '3818 C'],
        Np: ['Neptunium', '93', '237.0482', '640 C', '3902 C'],
        Pu: ['Plutonium', '94', '(244)', '639.5±2 C', '3235±19 C'],
        Am: ['Americium', '95', '(243)', '994 C', '2607 C'],
        Cm: ['Curium', '96', '(247)', '1340 C', 'N/A C'],
        Bk: ['Berkelium', '97', '(247)', 'N/A C', 'N/A C'],
        Cf: ['Californium', '98', '(251)', 'N/A C', 'N/A C'],
        Es: ['Einsteinium', '99', '(254)', 'N/A C', 'N/A C'],
        Fm: ['Fremium', '100', '(257)', 'N/A C', 'N/A C'],
        Md: ['Mendelevium', '101', '(258)', 'N/A C', 'N/A C'],
        No: ['Nobelium', '102', '(259)', 'N/A C', 'N/A C'],
        Lr: ['Lawrencium', '103', '(260)', 'N/A C', 'N/A C']
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
