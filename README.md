# 02-Starting-Project
GitHub Actions - Basic Building Blocks &amp; Components

E stimulojm nje TEST Fail
Tek src/components/maincontect.test.jsx ne rreshtin 19

E ndrrojm nga: expect(screen.getByTestId('help-area')).toBeInTheDocument();

Ne problem te ri: expect(screen.getByTestId('help-area')).not.toBeInTheDocument();

E bajm nje commit te ri edhe new workflow

E kam kriju nje workflow te ri,  deployment.yml  i njejt sikur me lart por me dy jobs inside, qe jan paralele.
Detyra e radhes asht me i nda tani ne paralele edhe me ba trigger Events

Sequential jobs, bahen me psh  needs:test shih fajllin sequential-deployment.yml

Qysh e testojm sequntial jobs, e bajm break prap ne rreshtin 19, sikur me lart

Disa sequential jobs  on: [push, workflow_dispatch]

Disa Expressions and Outputs me github:  run: echo "${{ toJSON(github) }}"
