<template>
    <Head>
        <Title>PrimeVue - Pass Through</Title>
        <Meta name="description" content="The Pass Through attributes is an API to access the internal DOM Structure of the components." />
    </Head>
    <div class="doc">
        <div class="doc-main">
            <div class="doc-intro">
                <h1>Pass Through</h1>
                <p>The Pass Through attributes is an API to access the internal DOM Structure of the components.</p>
            </div>
            <DocSections :docs="docs" />
        </div>
        <DocSectionNav :docs="docs" />
    </div>
</template>

<script>
import BasicDoc from '@/doc/passthrough/BasicDoc.vue';
import CustomCSSDoc from '@/doc/passthrough/CustomCSSDoc.vue';
import DeclarativeDoc from '@/doc/passthrough/DeclarativeDoc.vue';
import GlobalDoc from '@/doc/passthrough/GlobalDoc.vue';
import IntroductionDoc from '@/doc/passthrough/IntroductionDoc.vue';
import LifecycleDoc from '@/doc/passthrough/LifecycleDoc.vue';
import PCPrefixDoc from '@/doc/passthrough/PCPrefixDoc.vue';
import UsePassThroughDoc from '@/doc/passthrough/UsePassThroughDoc.vue';

export default {
    data() {
        return {
            docs: [
                {
                    id: 'introduction',
                    label: 'Introduction',
                    component: IntroductionDoc
                },
                {
                    id: 'basic',
                    label: 'Basic',
                    component: BasicDoc
                },
                {
                    id: 'declarative',
                    label: 'Declarative',
                    component: DeclarativeDoc
                },
                {
                    id: 'pcprefix',
                    label: 'PC Prefix',
                    component: PCPrefixDoc
                },
                {
                    id: 'lifecycle',
                    label: 'Lifecycle',
                    component: LifecycleDoc
                },
                {
                    id: 'global',
                    label: 'Global',
                    component: GlobalDoc
                },
                {
                    id: 'customcss',
                    label: 'Custom CSS',
                    component: CustomCSSDoc
                },
                {
                    id: 'usepassthrough',
                    label: 'UsePassThrough',
                    component: UsePassThroughDoc
                }
            ]
        };
    }
};
</script>
