# Lab 3  
## `grep` command options  

### Option 1: `grep -v`  

`grep -v` does a reverse search on the argument instead of a regular search.  
  
Example 1  
`grep what */*/5_Legal_Groups.txt`  
showed  
`what was already there. The hardwood floors, wooden ceilings and`  
while  
`grep -v what */*/5_Legal_Groups.txt`  
showed  
```5 Legal Groups at 1 Locale To Serve the February 3, 2002
Vulnerable
Salt Lake City Tribune
BY EDWARD MCDONOUGH
Five independent Salt Lake organizations that provide legal
services to the poor, ethnic minorities, seniors and people with
disabilities have joined together to acquire a west-side downtown
building where they will have their offices. The new Community
Legal Center at 205 N. 400 West is a project of "And Justice for
All," which, until this venture, has been a joint fund-raising
campaign by an alliance of the non-profit providers of free legal
services. "And Justice for All," which solicits donations primarily
from Utah lawyers and foundations, was the first joint fund-raising
campaign of legal services agencies in the country, and the
Community Legal Center is the first joint office project of public
service law groups.
The Legal Aid Society of Salt Lake, the Disability Law Center,
the Multi-Cultural Legal Center, the Senior Lawyer Volunteer
Project and Utah Legal Services will share the new facility, and
last Wednesday their board members were given a tour of the
Community Legal Center hosted by staff members of the five
agencies. All of the agencies can share the same reception area and
client waiting room. The building is close in, across the street
from West High and two blocks from the Gateway. It has its own
parking, something that's hard to find downtown and which has been
a problem for staff as well as clients. Owning and sharing the
building and not paying rent times five will save the non-profit
agencies about $375,000 each year. My assistant, Charity
Christenson, pointed out that the shared facility will also be
efficient for those needing legal services. No longer will a woman
desperate for a protective order, for example, have to run all over
town trying to find the right agency.
After the tour, we found Jaye Olafson at the cookies and
brownies reception on the first floor. Jaye and her husband, Erik,
own Tomax Technologies and were the sellers of the building. Jaye
explained how much of the renovation had been merely uncovering
brick and stone interior walls were all hidden behind coverings and
old paint. She loves the building, and they only moved out because
the business had outgrown the space. So they renovated the old
Sweet Candy Company building for Tomax. The Olafsons are delighted
with the new owners. The building had been like home, she
explained, and so it was important who would be living there. I
noted on the donor list that the couple, through Olafson Group, had
become one of the major supporters of the project.
Stewart Ralphs, the executive director of the Legal Aid Society,
explained that the Community Legal Center Campaign still has a long
ways to go, with a bit more than half of the $4 million projected
cost received so far. There still needed to be furnishings and
office equipment and such. He promised that they would be getting
in touch with us later on the subject.
```
  
Example 2  
`grep -v "For people" */*pbio.0020040.txt`
showed  
```       half of the 1990s, everything looked simple and straightforward. It was the stuff you could
        explain to sincerely interested relatives who wanted to know what you were spending your
        time on. There were oncogenes and there were tumour suppressor genes. Oncogenes were
        overactive genes and proteins that somehow caused cancer because they were overactive;
        therefore, they were dominant. Tumour suppressor genes were genes that would normally
        prevent a tumour from happening and that needed to be inactivated for a tumour to start to
        form; both copies of a tumour suppressor gene had to be inactivated, and the mutation was
        recessive. If inactivation of these genes is a random process, it was understandable that
        people who inherit an inactivated copy of a tumour suppressor gene had a higher risk of
        developing the associated form(s) of cancer than people born with two normal copies, as
        postulated in Alfred Knudson's (1971) two-hit model. And, indeed, it was shown that in the
        tumours in these predisposed patients, the remaining wild-type copy of the tumour
        suppressor gene was lost, a process referred to as loss of heterozygosity.
        For me, in 1998 things started to change. Venkatachalam et al. (1998) published a paper
        in the
        EMBO Journal describing a detailed study of tumours in mice lacking one
        copy of the p53 tumour suppressor gene (
        Trp53 ). This gene is known to be the most mutated gene in human cancer
        and its function to be central to many processes that are involved in the cellular
        prevention of cancer. Mice lacking both copies of this gene are for the most part viable,
        but succumb to cancer (mainly thymic lymphomas) at three to five months of age (Donehower
        et al. 1992). Mice born with one copy of the
        Trp53 gene start to develop cancer at around nine months, and incidence
        increases with age.
        In their study, Venkatachalam and colleagues analysed an impressive group of 217
        Trp53
        +/− mice of controlled genetic background and followed the fate of the
        Trp53 wild-type allele in the tumours. According to the two-hit model, it
        was expected that in these tumours this copy would have been lost or inactivated. However,
        this turned out not to be the case. Half of the tumours from mice younger than 18 months
        were found to have retained the wild-type copy of
        Trp53 , a number that increased to 85% in mice older than 18 months. In
        two tumours, the researchers sequenced the complete coding region of the remaining
        wild-type allele and showed it was structurally intact. To exclude the possibility of
        downregulation or inactivation at the level of protein expression, they irradiated
        tumour-bearing mice prior to sacrifice, a treatment known to increase p53 protein levels
        via posttranslational mechanisms. Their data showed the retained wild-type allele in these
        tumours was expressed normally and suggested it had a normal wild-type conformation.
        Next, the authors did a rigorous test of different functions of the p53 protein. They
        first tested whether the tumours showed amplification of Mdm2. This protein, whose
        expression is regulated by p53, stimulates breakdown of p53, thereby forming a negative
        feedback mechanism that keeps p53 levels low. Some tumours therefore amplify the
        Mdm2 gene as a means of inactivating p53. However, this was not found in
        the tumours from the
        Trp53
        +/− mice. Subsequently, the researchers tested to what extent the
        retained 
        Trp53 copy behaved normally. Irradiation of many tissues leads to
        p53-dependent apoptosis, and, indeed, in tumours that had retained the wild-type allele,
        irradiation did lead to an increase in apoptosis, whereas in tumours that had lost the
        wild-type allele, it did not.
        The p53 protein is known to function as a transcriptional regulator by either up- or
        down regulating target genes in response to different forms of cellular stress, including
        irradiation-induced DNA damage. The authors studied the expression of two p53-upregulated
        genes (
        Cdkn1a , which encodes p21, and
        Mdm2 ) and one downregulated gene (
        Pcna ) in p53-positive tumours after irradiation and showed responses
        indicative of normal p53 function. Furthermore, it was shown that the p53 protein from the
        tumours was able to bind to a p53-binding DNA sequence in an in vitro setting. Finally,
        since it is known that p53 absence in tumours is correlated with chromosomal instability,
        Venkatachalam et al. (1998) used comparative genome hybridisation to compare this feature
        between p53-negative and p53-positive tumours and found a 5-fold greater stability in the
        latter.
        In short, this paper clearly showed that, at least in mice, in many
        Trp53
        +/− tumours the wild-type allele of
        Trp53 is not only retained, but also appears to function normally. This
        strongly suggested that a decrease of dosage in p53 is already sufficient for
        tumourigenesis, a phenomenon referred to as haploinsufficiency. Shortly before, the group
        of Moshe Oren (Gottlieb et al. 1997) had shown that a
        Trp53
        +/− background leads to a greater than 50% reduction in p53 activity
        using a p53-responsive
        lacZ reporter gene in transgenic mice. Venkatachalam and colleagues
        suggested the strong concentration dependence of p53 function could be explained by the
        fact that p53 functions as a tetramer. A 50% decrease in p53 monomers can easily be
        imagined to result in a greater than 50% decrease in functional tetramers, which in turn
        increases the chances of these cells becoming cancerous.
        This paper by Venkatachalam et al. (1998) made me realise how important it is to remain
        critical, even of long-established theories and models. Since then, haploinsufficient
        mechanisms have been described in more tumour suppressor genes in humans and mice (reviewed
        in Fodde and Smits 2002). For instance, in a recent paper in
        PLoS Biology , Trotman et al. (2003) used mouse models to describe how
        the dosage of the
        Pten tumour suppressor gene influences the occurrence of prostate cancer.
        Further genes have been described with other unexpected roles in the tumourigenic process.
        There is a long-standing debate in the literature about the number and role of mutations in
        a tumour, and without going into the details, it is clear that haploinsufficient mechanisms
        for tumour suppressor genes will greatly influence the statistics on which these
        discussions are based. At a time when microarray analysis has become a standard experiment
        and the many thousands of changes in tumour cells are analysed across the whole genome, it
        is important to keep in mind that the correct interpretation of this wealth of information
        might be more complicated than the widely accepted models would have us believe.
        ```  
because "For people" was only included in the first line.  
`-v` could be a quick alternative for regex.  

### Option 2: `grep -h`  

`grep -h` displays only the lines that matched the argument and excludes the filenames.  

Example 1  
`grep "comments" */Post_Rate_Comm/*`  
showed  
```government/Post_Rate_Comm/Gleiman_gca2000.txt:comments some of you have been making, it appears that I didn't
government/Post_Rate_Comm/Gleiman_gca2000.txt:though, that most industry comments pale by comparison to some of
government/Post_Rate_Comm/Gleiman_gca2000.txt:Notwithstanding the comments of one of the Postal
government/Post_Rate_Comm/Gleiman_gca2000.txt:Despite the comments of a Governor concerning costs
government/Post_Rate_Comm/ReportToCongress2002WEB.txt:the comments of interested parties, implemented four of the
government/Post_Rate_Comm/ReportToCongress2002WEB.txt:comments of the Postal Service and other participants, the
government/Post_Rate_Comm/ReportToCongress2002WEB.txt:The Commission solicited two rounds of comments on the proposal
government/Post_Rate_Comm/ReportToCongress2002WEB.txt:Upon consideration of the initial comments it received, the
government/Post_Rate_Comm/ReportToCongress2002WEB.txt:solicited further comments on several broad issues concerning
```  
while  
`grep -h "comments" */Post_Rate_Comm/*`  
showed  
```comments some of you have been making, it appears that I didn't
though, that most industry comments pale by comparison to some of
Notwithstanding the comments of one of the Postal
Despite the comments of a Governor concerning costs
the comments of interested parties, implemented four of the
comments of the Postal Service and other participants, the
The Commission solicited two rounds of comments on the proposal
Upon consideration of the initial comments it received, the
solicited further comments on several broad issues concerning
```  
  
Example 2  
`grep -h "overview" government/About_LSC/*`  
showed  
`4) LSC - Michael Genz provided an overview of LSC's technology
overview)`  
instead of  
```government/About_LSC/conference_highlights.txt:4) LSC - Michael Genz provided an overview of LSC's technology
government/About_LSC/Progress_report.txt:overview)
```  
`-h` can be useful if you only care about the lines that include the argument and not the files that include the lines.  

### Option 3: `grep -c`  

`grep -c` displays the number of matching lines instead of the content of the lines.  
  
Example 1  
`grep -c -v "For people" */*pbio.0020040.txt`  
showed  
`105`  
which is the number of lines in the second example of option 1.  
  
Example 2  
`grep -c "comments" */Post_Rate_Comm/*`  
showed  
```government/Post_Rate_Comm/Cohenetal_comparison.txt:0
government/Post_Rate_Comm/Cohenetal_Cost_Function.txt:0
government/Post_Rate_Comm/Cohenetal_CreamSkimming.txt:0
government/Post_Rate_Comm/Cohenetal_DeliveryCost.txt:0
government/Post_Rate_Comm/Cohenetal_RuralDelivery.txt:0
government/Post_Rate_Comm/Cohenetal_Scale.txt:0
government/Post_Rate_Comm/Gleiman_EMASpeech.txt:0
government/Post_Rate_Comm/Gleiman_gca2000.txt:4
government/Post_Rate_Comm/Mitchell_6-17-Mit.txt:0
government/Post_Rate_Comm/Mitchell_RMVancouver.txt:0
government/Post_Rate_Comm/Mitchell_spyros-first-class.txt:0
government/Post_Rate_Comm/Redacted_Study.txt:0
government/Post_Rate_Comm/ReportToCongress2002WEB.txt:5
government/Post_Rate_Comm/WolakSpeech_usps.txt:0
```  
which is the number of matching lines in each file under the "Post_Rate_Comm" folder.
`-c` can be useful if we intend to do some sort of calculation with the number of matching lines, such as getting the ratio of matching and non-matching lines.  

### Option 4: `grep -n`

`grep -n` displays the matched lines along with the line numbers.
  
Example 1  
`grep -n "overview" government/About_LSC/*` 
showed  
```government/About_LSC/conference_highlights.txt:244:4) LSC - Michael Genz provided an overview of LSC's technology
government/About_LSC/Progress_report.txt:606:overview)
```  
which is the second example of option 2 including the line number of the matching lines.  
  
Example 2  
`grep -n "comments" government/Post_Rate_Comm/ReportToCongress2002WEB.txt`  
showed  
```257:the comments of interested parties, implemented four of the
425:comments of the Postal Service and other participants, the
447:The Commission solicited two rounds of comments on the proposal
459:Upon consideration of the initial comments it received, the
461:solicited further comments on several broad issues concerning
```  
which showed all the matching lines with the line number prepended to the beginning of each line.  
`-n` can be useful if you want to quickly navigate the file to get to the matching lines without using "ctrl + f".  

### References  
[WikiBooks] (https://en.wikibooks.org/wiki/Grep)  
[GeeksforGeeks] (https://www.geeksforgeeks.org/grep-command-in-unixlinux/)
