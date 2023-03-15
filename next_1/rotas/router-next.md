# Para criação de rotas
## Folder pages
`import Link from '../src/components/Link';

export default function <Name>Page() {
    return (
        <div>
            <Link href="/path">
                Description
            </Link>
        </div>
    )
}`

## Folder src/components/Link
`import NextLink from 'next/Link';

export default function Link({ children, href, ...props}) {
    return (
        <Link href={href} passHref>
            <a {...props}>{children}</a>
        </Link>
    )
}`



