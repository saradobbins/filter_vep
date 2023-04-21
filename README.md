# filter_vep

bcftools view joint_call_april_2023_split.joint-called.vcf.gz.anno.P2.vcf.gz -r chr4:165873237-166104457 -f PASS > TLL1.vcf

filter_vep -i TLL1.vcf -o stdout --filter "Impact is MODERATE" --filter "MAX_AF < 0.1 or not MAF_AF " --filter "CANONICAL is YES"



